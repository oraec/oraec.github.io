# ORAEC and Wikidata

Hi guys! Here we are again. We hope you had a great time. Our spiritual retreat did us a lot of good! But we are no longer in the same line-up as last year. Some are doing projects with [ChatGPT](https://chat.openai.com/chat) now, some are with [Exodus90](https://exodus90.com/). But we still produced (we hope) something useful. What is it about?

Well, we have a [controlled vocabulary](https://oraec.github.io/corpus/controlled_vocab.html) that is used in the metadata of the texts. For example, there is the term "Wadi Maghara" for a particular place, or "Unas" for a particular king. The [taxonomy we have adopted](https://github.com/simondschweitzer/aed-tei/blob/master/files/thesaurus.xml) uses German terms, but not English ones. This is, of course, awkward. Sure, we could have simply translated the terms now. But it seemed to make more sense to us to link them to an English controlled vocabulary. And now Wikidata comes into play.

What is [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page)? Wikidata is a sister project of Wikipedia. If Wikipedia is a wiki for an encyclopedia, Wikidata is a wiki for ..., well, what?, of course: for data. Wikidata has become the one-stop shop for referencing data of all kinds, for places, for institutions, for time periods, for people, in other words, for everything in our controlled vocabulary.

We have now gone through our controlled vocabulary and mapped the entries with Wikidata. [Here](https://github.com/oraec/corpus_raw_data/blob/main/mapping_oraec_wikidata.tsv) is our mapping as tsv file, of course licensed with cc0. On the web pages, we've added an additional section called "More info". There is now the link to the entry in Wikidata.

This has several advantages:

Now there are definitions to the entries through the link: Did you know the German word "Sturz"? This is the name of an entry in the controlled vocabulary: <https://oraec.github.io/corpus/YPVD27R3SBHPLJUFB5SJYAHBMQ.html> But if you don't know the word and look it up, you get the translation "fall". That can't be what is meant. The German word "Sturz" is ambiguous. Here it is "lintel". [Wikidata](https://www.wikidata.org/w/index.php?title=Q1370517&oldid=1764590714) defines the term as follows:

> structural horizontal beam that spans the space between two vertical supports above an opening

That helps, doesn't it?

Wikidata provides additional info about a term, sometimes even photos, and also the links to the Wikipedia articles.

But the best is: We have linked our controlled vocabulary to the central instance. This makes us part of the large network of "linked data". Have a look at the entries at Wikidata. They are linked to many other thesauri. So Wikidata allows cross-thesaurus research, now also with Egyptian texts. Yeah!

Do you think this is as cool as we do? Stay tuned. We want to offer you many more great things until Lent!
