# Next steps

Thank you very much for the many reactions to our project, especially the nice ones made us happy. Many great ideas have reached us. We want to report in this blog, which of them we want to implement and in which form:

## Hierarchy

Some of our text names are a bit cryptic. What does "Textfeld / Westwand (Aussen)" mean for [oraec46](https://oraec.github.io/corpus/oraec46.html)? That's already in [AED](https://simondschweitzer.github.io/aed/) and [AES](https://github.com/simondschweitzer/aes), which is not very user-friendly. Therefore we go back to the [data basis](https://nbn-resolving.org/urn:nbn:de:kobv:b4-opus4-29190). There, the individual data sets are arranged in a hierarchical tree. The text is child element of a wall, the wall is child element of a room, the room is child element of a tomb. We will extract this hierarchy for each text and make it available.

## Search interface

Unfortunately, we don't have a search interface and we won't have one in the foreseeable future. (Or is there someone out there who could build one for us?) The great idea of being able to search for synonyms of texts (Ipuwer, Admonitions) will unfortunately not be implemented. We also don't have a search interface for a word search. As a small help we want to create a list of all lemmas used in ORAEC.

## Collocations

As promised before, we will create collocations: when does lemma X appear together with lemma Y.

## Linked data

Many Egyptological projects offer digital data. Users can benefit if these projects are linked together. Most impressively, [Trismegistos](https://www.trismegistos.org/) implements this. If we count correctly, that's currently 159 projects linked by Trismegistos: <https://www.trismegistos.org/partners.php> Congratulations, colleagues! We will link our entries to Trismegistos first. After that, we will look at the museum databases.

## Collaboration with other projects

Other digital Egyptology projects have contacted us. Cooperations are planned. We will report more when there is something concrete.

## The nature of the character

Paleographically oriented research questions are immensely important. Paleography and epigraphy can be used to determine dating or provenance. However, such questions are to be separated from the approach, what is a character at all. We want to emphasize here again that we orient ourselves at Unicode. Thus we summarize allographs like W11 and W12 under one character.

## Data quality

With the large amount of data, errors naturally occur. For example, there is a Ḥw-mḥn in [oraec2](https://oraec.github.io/corpus/oraec2.html), which should correctly read Ḥrn. This affects the tokens [oraec2-170-7](https://oraec.github.io/corpus/oraec2-170.html) and [oraec2-177-2](https://oraec.github.io/corpus/oraec2-177.html). If we notice errors or if someone brings errors to our attention, we will correct them. We will probably bundle the corrections and publish a second version of the dataset at some point in the future.

## First of all
First, though, we're doing something unrelated to the core corpus. The great [AKU project](https://aku.uni-mainz.de/) has a nice [blog](https://aku.hypotheses.org/) that [most recently](https://aku.hypotheses.org/3063) reports on the use of Unicode in Egyptological transcription. The blog also refers to keyboards that create the transcription. We will next report on the various keyboards.
