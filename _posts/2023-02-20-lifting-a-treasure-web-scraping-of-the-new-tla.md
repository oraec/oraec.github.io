# Lifting a treasure - web scraping of the new TLA using the demotic corpus as an example

Do you remember? Last year, we reviewed the [new TLA](https://thesaurus-linguae-aegyptiae.de/). It was so detailed that we had to split the [review](https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html) into [four](https://oraec.github.io/2022/11/17/review-of-the-new-tla-part-four.html) parts. Roughly summarized, we came to the following conclusion: the data of the new TLA is excellent. However, the functionalities of the new TLA are rather poor. Apparently there was not enough time to implement important tools (e.g. the text view), because questionable things like superfluous wildcards, hard-coded hieroglyphic groupings or lemma comments with insufficient content were implemented. The new TLA has been online for more than 3 months. In December, the web app version 2.01 was released. There, some shortcomings that we had addressed in our review were also fixed, for example, the citation note now includes the author information, which - contradicting the CC-BY-SA license - was initially missing. After December, not much has happened on the Github repository. A bit scary is the following commit from December: <https://github.com/thesaurus-linguae-aegyptiae/tla-web/commit/0ccafbdce7a16b5ff3af8761ba98facfa3bb4cb7#> There the raw data publication is downgraded from high priority to medium priority. That means: the strength of the project, namely the actual data, will not be published at all yet. Other things are to be tackled first, such as the feedback form. Doesn't project management actually do a [SWOT analysis](https://en.wikipedia.org/w/index.php?title=SWOT_analysis&oldid=1138237844)? The central product, the [cash cow](https://en.wikipedia.org/w/index.php?title=Cash_cow&oldid=1134012372) of the TLA is simply the data. So much cool research could be done with that data, but as yet the data is locked up in the TLA.

How can one free the data from its prison? Before launching such a liberation operation, one must of course consider the legal dimension. Is this even allowed? Fortunately, the answer to this question is yes. The TLA licenses the scientific data under the CC-BY-SA license, cf. <https://thesaurus-linguae-aegyptiae.de/info/licenses>. If one considers the license conditions, one is allowed to free the data from its prison.

How to free data? The data is located on the domain <https://thesaurus-linguae-aegyptiae.de/> and is published on various HTML pages. This published data can be harvested. The procedure is called [web scraping](https://en.wikipedia.org/w/index.php?title=Web_scraping&oldid=1137141826). There are various tools that can be used. For example, there is a package for R, see [this introductory blog](https://statsandr.com/blog/web-scraping-in-r/). In our blog, we want to exemplify how to obtain the data from the new TLA. We want to extract all the demotic sentences of the TLA. To do this, we first search for all demotic lemmas in the TLA: <https://thesaurus-linguae-aegyptiae.de/search/lemma?_script=on&script=demotic&_script=on&transcription.text=&transcription.enc=unicode&wordClass.type=&root=&translation.text=&translation.lang=de&bibliography=> The TLA generates a hit list of 15255 demotic lemmas. Wow, the old TLA only had 12451 lemmas. That's a tremendous increase. Thank you, lexicographers, namely: Altägyptisches Wörterbuch, Theresa Annacker, Jakob Hoeper, Simon D. Schweitzer, Günter Vittmann, Anja Weber. We were also able to obtain these names with web scraping. But back to the demotic lemmas in the new TLA!

The hit list with the 15255 demotic words refers to the lemmas with hyperlinks. We collect all links to get a list of all demotic lemmas <https://github.com/oraec/scraped_data/blob/main/new_tla/demotic/ids_of_demotic_lemmata_in_the_new_tla.txt>. A detail page of a lemma has a link to the supporting documents of the lemma. Such a document page consists of different demotic clauses, where they are linked. Thus, we control each document page of each lemma and store each link to a demotic sentence. Since usually a demotic sentence consists of many demotic words, we get each demotic sentence multiple times. Of course, we list the same demotic sentence only once. We get a list of almost 30000 sentences in the new TLA: <https://github.com/oraec/scraped_data/blob/main/new_tla/demotic/ids_of_demotic_sentences_in_the_new_tla.txt> We cannot guarantee that this list contains every demotic sentence; because we can think of demotic sentences that do not contain any lemmatized word form. Look at the last sentence of the magic papyrus Vienna D 12006 in the old TLA: <https://aaew.bbaw.de/tla/servlet/GetCtxt?f=0&l=0&tc=5&db=1&ws=0&mv=5> There is only as indication of a destruction "vom_Rest_der_Kolumne_nur_dürftige_Reste". There is no lemmatized word here. Therefore, such a sentence cannot enter our list.

In addition to this list, which contains only the IDs of the sentences, we have evaluated something else. The page of a demotic sentence indicates to which text this sentence belongs. Thus we have assigned to the different demotic texts their corresponding sentences. This is in the following file: <https://github.com/oraec/scraped_data/blob/main/new_tla/demotic/demotic_sentences_in_the_new_tla.json> The object "text" contains as keys the demotic texts. The values are the demotic sentences. The new TLA does not publish the correct sequence of sentences. That is: we cannot reverse engineer the sequence of sentences within a text with the published data alone. Nevertheless, already the information which sentences a text has is useful for corpuslingusitic research. Often, one only evaluates a [bag of words](https://en.wikipedia.org/w/index.php?title=Bag-of-words_model&oldid=1137265046) anyway, disregarding the order.

In addition to the texts, we have also evaluated the dating of the sentences. On a detail page of a sentence, not only is the dating given, but there is also a link to the corresponding thesaurus entry. The thesaurus entries can be looked up directly in the new TLA or conveniently found in AED-TEI: <https://github.com/simondschweitzer/aed-tei/blob/master/files/thesaurus.xml>. The TLA now uses two types of dating. Either one thesaurus entry is referenced or two are referenced to indicate an interval. Thus, the TLA dates the record <https://thesaurus-linguae-aegyptiae.de/sentence/IBUBdwMhNYGC40H7rCTiAE6UQLM> to the period from the 27th dynasty to the 31st dynasty. In our file <https://github.com/oraec/scraped_data/blob/main/new_tla/demotic/demotic_sentences_in_the_new_tla.json>, we have the keys ``date`` and ``date_range`` for these two types. In the object belonging to ``date`` we find as keys the IDs of the dating thesaurus entries and as associated values all the records that are dated with this dating specification. I.e. all records from the 26th dynasty are gathered in one place! For interval dating, we specify the two IDs separated by a ``|``. So the above example sentence IBUBdwMhNYGC40H7rCTiAE6UQLM is found at the key "2AVEQ3VFT5EEPF7NBH7RHCVBXA|2Z7FB3JW3BHGRPWOII5PAYY4DM", because 2AVEQ3VFT5EEPF7NBH7RHCVBXA is the ID for the 27th dynasty and 2Z7FB3JW3BHGRPWOII5PAYY4DM is the ID for the 31st dynasty. This sorting of demotic sentences based on dating allows for a focused study of the various chronolects of demotic. Commonly, one differentiates between the early, the ptolemaic and the roman demotic. With this pre-sorting, one can thus create a corpus of the demotic of a certain time stage.

By the way, the oldest demotic sentence - hopefully this fun is allowed - is from the Heracleopolitan period: <https://thesaurus-linguae-aegyptiae.de/sentence/IBUBd4VNTRcpvUWvtwhBm3psfn4> This is a sentence from a letter of the first intermediate period. Why does our web scraping find this sentence? Only demotic lemmas are searched. There is a small error here. Let's see what's going on: this sentence is also in the ORAEC corpus: <https://oraec.github.io/corpus/oraec3176-1.html>. The token oraec3176-1-8, the written form mj-jḫ, has been split into two elements for the new TLA. The first element, the preposition mj, has now been incorrectly linked to the entry in the demotic word list. Thus, this sentence is an occurrence for the demotic preposition mj. And therefore this sentence is found by web scraping.

Back to the right analysis! With the liberated data, we can also do quantitative analysis. We counted the records the TLA contains for each of the three chronolects:

| chronolect  | sentences in the new TLA |
| ------------- |:-------------:|
| early demotic      | 3170     |
| ptolemaic demotic      | 13966     |
| roman demotic      | 11187     |

Thus, most of the sentences are from the ptolemaic period, followed closely by those from the roman period. The early demotic sentences are significantly fewer. Is this distribution representative? Representative means that the linguistic features in a corpus adequately reflect the proportions of the (statistical) population without overemphasizing or neglecting the individual parameters. The pre-demotic corpus in the old TLA, for example, is not representative. The pyramid texts distort the distribution, so that the six most frequent royal names got their front position only because of the pyramid texts. <https://aaew.bbaw.de/tla/servlet/s0?f=0&l=0&ff=8&ex=1&db=0&oc=1&wt=6&l1=0&mx=10> In other words, the fact that the name Ramesses is not in the top ten does not reflect the real distribution, but is due to the text selection. Even if only a fraction of all texts are included in a corpus, this corpus can still be representative.

> A corpus may be small but more representative of a language, variety or register than larger ones if sampling is based on systematic, linguistically-motivated decisions rather than convenience or some principle of authority, as was perhaps often the case with first-generation corpora. (Raineri, S. & Debras, C. (2019). Corpora and Representativeness: Where to go from now?. In CogniTextes 19. URL: <http://journals.openedition.org/cognitextes/1311>; DOI: <https://doi.org/10.4000/cognitextes.1311>)

Günter Vittmann, the main author of the demotic corpus in the TLA, described his selection criteria in an article:

> Aus diesem Bestreben heraus, aber gleichzeitig motiviert durch die Absicht, eine möglichst große Anzahl lexikalisch, phraseologisch, grammatisch und inhaltlich ergiebiger Texte der verschiedensten Gattungen aufzubereiten, werden – ohne eher formelhafte Dokumente mit notorisch repetitiven Elementen zu vernachlässigen – bevorzugt Texte ausgewählt, die in irgendeiner Weise etwas Besonderes zu bieten haben. Während man bei der großen Masse von Rechtsurkunden und Verwaltungsdokumenten, wie schon angedeutet, mit einer repräsentativen Auswahl, bei der der Benutzer zwangsläufig dieses oder jenes vermissen wird, vorliebnehmen muss, sind bestimmte Textgattungen des demotischen Schrifttums dazu prädestiniert, soweit der aktuelle Publikationsstand dies erlaubt, in besonders hohem Umfang aufgenommen zu werden[.] (Vittmann, G. (2013). Zur Arbeit an der Demotischen Textdatenbank : Textauswahl. In Hafemann, I. (ed.). Perspektiven einer corpusbasierten historischen Linguistik und Philologie : Internationale Tagung des Akademienvorhabens „Altägyptisches Wörterbuch“ an der BBAW, 12.-13. Dezember 2011 (Thesaurus Linguae Aegyptiae 4). p. 146; URL: <https://nbn-resolving.org/urn:nbn:de:kobv:b4-opus-24370>)

With our counts, we now have a basis for making distributional considerations (cf. Egbert, J., Biber, D., & Gray, B. (2022). Corpus Representativeness: A Conceptual and Methodological Framework. In Designing and Evaluating Language Corpora: A Practical Framework for Corpus Representativeness (pp. 52-67). doi:10.1017/9781316584880.003) about the extent to which the demotic corpus in the new TLA is representative.

[Trismegistos](https://www.trismegistos.org/lang/detail.php?language_id=21) provides the statistical function of counting the demotic texts treated there by dating in the collection period of Trismegistos, that is, from the 8th century BC to the 8th century AD. It results:

| centuries  | demotic texts in Trismegistos |
| ------------- |:-------------:|
| eighth century BC - fourth century BC      | 2265     |
| third century BC - first century BC      | 5797     |
| first century AD - eighth century AC      | 3397     |

Of course, the periods are not congruent. The TLA offers the period [4. Viertel 1. Jhdt. v.Chr.](https://thesaurus-linguae-aegyptiae.de/thesaurus/3V5NOJIC3VBIZBA7QCD6OFSAQY), which we can count in our enumeration to the roman period, but which must necessarily be assigned to the second period by Trismegistos. Nevertheless, it is noticeable that the distributions are different. According to the TLA, ptolemaic and roman demotic stand out from the early, while according to Trismegistos rather the early and roman demotic form a group and the ptolemaic demotic is to be separated from it. So do such distribution considerations now argue that the demotic corpus in the new TLA is rather unrepresentative? Or is it representative after all because of what Egbert, Biber, and Gray call domain considerations? It's a great research question, isn't it? Only the liberation of the data made it possible to ask it, and these data also provide the material to answer it.

People, use the data! They are intended for reuse; because they are licensed in this way! As you can see, you can ask great questions with it. And web scraping is not hard at all. So get started! We are not here in the near future! Lent is coming up. That means fasting, praying, and we'll be doing without the digital! See you after Easter!

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a></p>