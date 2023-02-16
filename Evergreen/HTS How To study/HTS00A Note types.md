---
reference: "[[Own Idea]]"
date: 07/01/2023
type: 1 #evergreen
topics: autodidact
aliases: HTS00A, Note Types, Notes
tags: how_study, guide, zettelkasten
code: HTS00A
---
# HTS00A Note types

The Zettelkasten[^1] method has three types of note, fleeting, literature and permanent notes. I only use two types of note and I'll name it in a different way. The notes are [[#00A.1 Source Notes|source notes]] that is like a kind of literature note, but no only for books and articles. And the other type is the [[#00A.2 Evergreen Notes|evergreen notes]], the latter is like the permanent note.

I don't use fleeting notes 'cause at present time there are so much tools to  write or record and save little thinks, ideas, or other things that could evolve in a Source Note. It could be Telegram, Whatsapp or the Note app of the phone.

# HTS00A/1 Source Notes

In these notes are placed the source of the information a summary of it in own words, if the quote text is short you can put  and all the relevant information from the source. these are not inside the zettelkasten system are saved to not lose the source information.

I use the metadata of obsidian to manage this notes. The template of the metadata is the next:
~~~ YAML
title: the title of the book | source
source: chapter, page, link, time, etc
author: Who is the author
date: automatically created
type: 2 #sourcenote is the type of the note.
topics: the topics of the note
tags: could be the same of the topics, but could not be it 
~~~
# HTS00A/2 Evergreen Notes

In the Evergreen notes is placed the processed information obtained from the [[#HTS00A/1 Source Notes|source notes]] and must follow two important rules:

1. It must be atomic, i.e., Each note only can have an idea, must be coherent, concise and brief and It must not repeat ideas from other notes. For this purpose I use a [[HTS00B Note Codes#HTS00B Note Codes|coding method]] to separate notes or ideas from other.
2. It must be connected to previous notes, because the brain always learn something new based on the known things, in the original zettelkasten the author wrote the codes in the pages, but with obsidian just need make a link to the note.

The metadata used for manage this type of note is the next:
~~~ YAML
reference: The link to the source note
date: automatically created
type: 1 #evergreen
topics: The topics of the note
aliases: aliases of the note
tags: the tags used to distinguish the note
code: the code of the note
~~~

# Links
<<[[HTS00 Guide|HTS00]]|[[HTS00B Note Codes|HTS00B]]>>

[^1]: [Zettelkasten](https://es.wikipedia.org/wiki/Zettelkasten)