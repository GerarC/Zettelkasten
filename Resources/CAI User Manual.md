# Manual de usuario de CAI

## Uso del Procesado de CSV

Para añadir nuevas bitácoras de manera más sencilla, se puede utilizar la opción de *subir csv bitácoras*. Ésta utilizará el archivo que se escoja para crear varias bitácoras al mismo tiempo sin tener que ingresar la información una por una.

### Formato del archivo

El formato que debe tener el archivo, obviamente, debe ser un csv y necesariamente la información tiene que estar separada por comas (los csv pueden separarse con otros símbolos).

Es obligatorio que las 6 del archivo columnas tengan el siguiente orden:
1. La primera columna debe tener la descripción de la bitácora.
2. La segunda el correo del auxiliar a la que será asignada.
3. La tercera tendrá el bloque en el que estará. Solo es necesario el número del bloque, exceptuando por el bloque 19 que se separa en *19 sur* y *19 norte* por lo cual en este caso se debe indicar justo como se acaba de escribir aquí.
4. La cuarta columna debe contener el piso en cuestión, también indicado solo con números. Por ejemplo *1*, *2*, *3*
5. La quinta será la fecha de la bitácora. El formato de esta fecha deber ser obligatoriamente `dd/mm/yyyy`, es decir, día, mes y año; solo los números. Por ejemplo *20/02/2025*.
6. Por última serán las horas de inicio y de final de la bitácora. El formato será `<hora inicio>-<hora final>`, donde `<hora inicio>` y `<hora final>` son números naturales entre *06* y *22*. 
	Por ejemplo, si un estudiante debe estar entre las 6AM y las 10AM en la bitácora se deberá escribir *06-10* o si debe de revisar entre las 4PM y las 6PM se usará *16-18*.
    
Un ejemplo de este formato hecho en **Google Sheets** puede ser:
![[Pasted image 20250204205108.png]]
    
Si desea descargar este archivo para que sea usado en *CAI* entonces debe dar click en donde se indica en la siguiente imagen:
![[Pasted image 20250204205031.png]]
    
Cuando lo descargue, si lo abre en el bloc de notas, debería verse así:
![[Pasted image 20250204211334.png]]
    
Una vez el archivo esté listo, se deberá subir en *CAI* para que sea procesado, esto se hará apretando el botón de **SUBIR CSV BITÁCORAS** localizado en la sección de asignar bitácoras al que pueden acceder los coordinadores y los auxiliares de oficina:
![[Pasted image 20250204210916.png]]
    
Se seleccionará el archivo dándole click al botón de browse y ya escogido se dará click al botón de **PROCESAR ARCHIVO**:
![[Pasted image 20250204210802.png]]

Si el archivo subido no tiene mal ningún formato y si nada más sale mal, tendría que ser mostrado el siguiente mensaje:
![[Pasted image 20250204210842.png]]