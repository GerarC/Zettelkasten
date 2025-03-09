# Archlinux Installation

## 1. Download Archlinux ISO
You can download it from [Archlinux Official Page](https://archlinux.org/download/), It has various options from Torrent to HTTP. Choose what you want.

## 2. Choosing Medium to install
If you will use VM or Physical Device

## 3. Installation Process

### 3.1. **Select keyboard layout**
To work in a easier way, you can set your keyboard layout to one you're used to use.
1. `localectl list-keymaps`: List available keyboards
2. `loadkeys <name>`: set keyboard layout

### 3.2. **Connect internet**
You have to verify and assure you can access to internet because the whole installation process need a connection.
1. `ping archlinux.org`: verify if you can access to internet.
2. `iwctl device list`: list WiFi cards.
3. `iwctl --passphrase <password> station <WiFi_card> connect <SSID>`

### 3.3. **Disk Partition**
1. `fdisk -l`: list available disks and their partition
2. `cfdisk <disk>`: command to make partitions.
   - For BIOS you should make at least _/_ and _/boot_ partitions
   - For UEFI you should make at least _/_ and _/boot/efi_ partitions
3. `mkfs.ext4`: format partition as ext4
4. `mkfs.ext2`: format boot partition in BIOS
5. `mkfs.vfat -F32`: format boot partition in UEFI

### 3.4. **Disk mount**
Once partitions are created and formatted, you must mount them so use the next commands
1. `mount /dev/<root_partition> /mnt`
2. `mount --mkdir /dev/<boot_partition> /mnt/<boot_dir>` where `<boot_dir>` can be _boot_ or _boot/efi_.
3. mount home and other partitions you made.

### 3.5. **Base packages**
1. `pacstrap -K /mnt linux linux-firmware base neovim dhcpcd networkmanager grub`: Install base packages.
   - _linux:_ kernell package
   - _base:_ base applications like `ls`, `cat`, `cd` and more
   - _neovim:_ text editor
   - _dhcpcd:_ dhcp demon
   - _networkmanager:_ self explanatory
   - _grub:_ Os chooser
   
### 3.6. **Gen FsTab**
**Fstab** or **File Systems Table** is a file that contains how are mounted all system partitions. Isn't automatically generated so, it's need create it.
- `genfstab -U /mnt >> /mnt/etc/fstab`: Generates fstab and append it into fstab file

### 3.7. **Enter as Root**
Now we need to enter into the installed to make some configurations.
- `arch-chroot /mnt`: Enters into the installation

### 3.8. **Configuration**
1. `ln -sf /usr/share/zoneinfo/<Region>/<City> /etc/localtime`: makes a Symbolic link from the city into localtime.
2. `hwclock --systohc`: configures the hardware clock.
3. Edit _/etc/locale.gen_, uncomment your language, in this case ==es_CO.UTF-8==, then execute `locale-gen` command.
4. create _/etc/locale.conf_ and put inside what you've just uncommented, i.e. `LANG=es_CO.UTF-8`.
5. create _/etc/vconsole.conf_ and set inside the keyboard layout that you set at the beginning, i.e. `KEYMAP=la-latin1`.
6. create _/etc/hostname_ and put inside the name you want for the computer in the network.

### 3.9. **Grub installation**
1. >
   > ##### UEFI
   > - `grub-install --efi-directory=/boot/efi --bootloader-id=<custom_id> --target=x86_64-efi`
   > ##### BIOS
   > - `grub-install /dev/<hard_disk>`
2. `grub-mkconfig -o /boot/grub/grub.cfg`
3. It's should be not necessary, bu you can use `mkinitcpio -P` to create initramfs

### 3.10. **Admin Password and First User**
1. As you should be admin, you can set an admin password with `passwd`
2. To create a user you can use `useradd -m <username>` and set password with `passwd <username>`.

### 3.11. **Reboot**
At this point base installation has finished, so it's we should reboot
1. `exit`: exit from `arch-chroot`.
2. `umount -R /mnt`
3. `reboot`

## 4. Post Configurations

### 4.1. Enable Network Manager
1. `systemctl enable NetworkManager.service`: allow to the service init with the OS.
2. `systemctl start NetworkManager.service`: starts network manager immediately.
#### 4.1.1 **Enable  WiFi**
3. `ip link set <wifi_card> up`: activates WiFi connection card
4. `nmcli dev wifi connect <SSID> password <password>`

### 4.2 Graphical Driver
1. `lspci | grep VGA`: find what type of VGA you have.
2. Install the driver with`pacman -S xf86-video-<driver>`, where `<driver>` can be `vesa` or `ati` or `nouveau`.

### What is GPT, MBR and what's the difference between both of them?

#### GPT
**GPT** or **GUID Partition Table** is a layout of the partition table of a hard drive that make uses of UEFI stuff. incompatible with BIOS. Creates a header and a footer to locate partition through a table.

> [!note]
> GUID and UUID is the same thing, and it means Globally Unique Identifier

#### MBR

**MBR** or **Master Boot Record** makes use of BIOS stuff, incompatible with GPT, It's used in Legacy hardware and firmware. Locates partition location at the beginning of the hard drive