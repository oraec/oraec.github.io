# Egyptian-UJaen, a treebank for the Pyramid Texts

Do you know what a treebank is? According to [Wikipedia](https://en.wikipedia.org/w/index.php?title=Treebank&oldid=1305280731):

> In linguistics, a treebank is a parsed text corpus that annotates syntactic or semantic sentence structure. The construction of parsed corpora in the early 1990s revolutionized computational linguistics, which benefitted from large-scale empirical data.

A [treebank for Coptic](https://universaldependencies.org/cop/index.html) has been published by the [Coptic Scriptorium](https://copticscriptorium.org/). The data is annotated according to [Universal Dependencies](https://universaldependencies.org/) rules, enabling exploration of the texts according to their syntactic properties. It is an invaluable resource for anyone interested in the Coptic language. As the name suggests, Universal Dependencies are cross-linguistic annotation rules. Therefore, if someone is familiar with these annotations, they can search the Coptic treebank and obtain results even if they don't know Coptic. Furthermore, Universal Dependencies make it possible to search for specific patterns in various languages, whether ancient or modern. If you want the field of general linguistics to take note of a particular language, you should annotate it with Universal Dependencies, just as the Coptic Scriptorium has done with Coptic.

Do you know of a treebank for Earlier Egyptian? No? Neither did we until we stumbled upon the [Egyptian-UJaen treebank](https://universaldependencies.org/treebanks/egy_ujaen/index.html), which describes itself as follows:

> Egyptian-UJaen is the first dependency treebank created for the morphosyntactic annotation of pre-Coptic Egyptian. Its current state (UD v2.17) consists of 2,347 sentences and 24,375 tokens manually annotated from texts written in Old Egyptian, mainly from the Pyramid Texts. ([Readme on Github](https://github.com/UniversalDependencies/UD_Egyptian-UJaen))

Have you seen any announcements? As far as we know, nothing has been published in the usual sources of information about this. It's unfortunate because it's an excellent resource for researching Egyptian. This treebank was presented at a [treebank conference in December 2024](https://www.korpuslab.uni-hamburg.de/en/tlt2024.html), as revealed in a [conference paper](https://aclanthology.org/2024.tlt-1.1/). The paper explains annotation guidelines such as transliteration, tokenization, lammatization, part-of-speech tagging, morphological analysis, UD relations, and hieroglyphs. Traditional transliteration uses an idiosyncratic approach that confuses Semiticists when comparing Egyptian to a Semitic language. This is why the treebank uses the Tübingen transcription system, writing "č̣" instead of "ḏ," for example. Here is a quote from the paper:

> Some colleagues attending the 13th International Conference of Egyptologists held in Leiden from 6 to 11 August 2023 established the Leiden Unified Transliteration (LUT),[fn.7] and there has been constant pressure since then to adopt it for the transcription of Egyptian texts in digital resources, text editions and publications. However, the LUT is clearly a scientific regression, as it keeps traditional signs, such as ṯ and ḏ, which were adopted in the 19th century only for typographical reasons. (p. 3)

Lemmatization reduces a word to its base form but does not use IDs that could disambiguate homonyms. Therefore, the lemmatization of 𓁷 is always ḥr, regardless of whether it is the preposition or noun. Hieroglyphs are annotated as Unicode hieroglyphs. Unfortunately, our [recommendations](https://oraec.github.io/2022/09/28/recommendations-encoding-hieroglyphs.html) are not taken into account. Positioning is annotated using [MdC](https://en.wikipedia.org/w/index.php?title=Manuel_de_Codage&oldid=1012543887) characters : and *. This is problematic for searches, especially since the positioning is artificial; it is based on Kurt Sethe's edition, which converted the original columns into lines. See below for hieroglyphs! The highlight of the annotation is the syntax, which is reproduced in the UD Relations. You may come across details that differ from other approaches. Is the verb in mḥ-jb n.j nzw ḫnti̯ =f really an adordination to mḥ-jb, as postulated on page 7? Or is the verb rather the root, with mḥ-jb as a front extension, as is so common in Egyptian grammar?

Nevertheless, we fully agree with the conclusion's words, which we quote below:

> When Joris F. Borghouts published his Middle Egyptian grammar in 2010, with a large number of examples and references to Egyptian texts, Wolfgang Schenkel predicted that a digital database of syntactically analysed sentences would be the next step in Egyptian philology. [fn. 20] The EUJA treebank makes Prof. Schenkel’s prediction come true, as it contains morphosyntactically annotated sentences from the most representative texts of each pre-Coptic stage. It will be an auxiliary tool for the study of Egyptian grammar, facilitating the synchronic and diachronic parsing of structures and words. (p. 8)

But how do you search a treebank? The Egyptian-UJaen treebank has its own web application: [GrewPT](https://grew.fr/grew_match/pt/)! Now, you can search the treebank using a query language. A query language is a powerful tool that can perform much better searches than a predefined web form. Unfortunately, using a query language is not very user-friendly. You must know the special syntax and avoid typos; otherwise, you won't get any results. Fortunately, there are several links on the left that simplify the search process. The first link is called "Search for a form." Then, fill in the search field.

![GrewPT Search for a form](/img/blog/grewpt_search_for_a_form.png "GrewPT Search for a form")

Instead of "Form_to_search," enter the desired transliteration and click "Search." There are 260 results.

![GrewPT Search for a form - hitlist](/img/blog/grewpt_search_for_a_form_hitlist.png "GrewPT Search for a form - hitlist")

The desired element is highlighted. The graphical representation of the relations in a tree is very informative, which is why it is called a "treebank."

![GrewPT Search for a form - hit](/img/blog/grewpt_search_for_a_form_hit.png "GrewPT Search for a form - hit")

The central element of the sentence is the root, on which all the other parts depend. In this example, it is the verb ꜣgbgb. The subject jb is connected to the root with the relation nsubj. The individual elements of the sentence are represented by their transliterations. Further information in the form of key-value pairs is provided below. These pairs are self-explanatory. What could "Number=Sing" mean?

Now here's an example of how powerful this treebank is. In this example, jb was the subject of the sentence. We can search for sentences where this is the case! Pretty cool, right? To do this, we simply enter "pattern { X[lemma="ꞽb"]; Y -[nsubj]-> X; }" in the search box and click on "Search":

![GrewPT Search for jb as subject](/img/blog/grewpt_search_jb_as_subject.png "GrewPT Search for jb as subject")

Of course, you have to learn a little bit of the query language, but it's worth it to unlock this treasure trove! Many thanks to Roberto Antonio Díaz Hernández for annotating the treebank and to Bruno Guillaume for programming the web application. Egyptological linguistics now has an excellent new tool!

Earlier, we discussed the annotation of hieroglyphs. We converted the hieroglyphs in this treebank according to our recommendations and integrated them into our [meta search engine](https://oraec.github.io/corpus/search/search_hieroglyphic_word_forms.html). Now, when you search for a hieroglyphic spelling such as "mr-r-n," you will also get results from this treebank.

![GrewPT Search for hieroglyphic word forms](/img/blog/grewpt_search_for_hieroglyphic_word_forms.png "GrewPT Search for hieroglyphic word forms")

A hit in GrewPT includes the sentence ID (EUJA-914) and the paragraph from Sethe's edition (§ 281b). The link leads directly to the sentence with the spelling in question.

![GrewPT Search for hieroglyphic word forms - hit](/img/blog/grewpt_search_for_hieroglyphic_word_forms_hit.png "GrewPT Search for hieroglyphic word forms - hit")

As you can see, the spelling is found even though the treebank annotates parentheses and colons. Have fun with our [meta search engine](https://oraec.github.io/corpus/search/search_hieroglyphic_word_forms.html) and, above all, with this great [treebank](https://pt.grew.fr/?corpus=PT_all)!

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a></p>
