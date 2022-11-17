# Review of the new TLA - Part four

This is the last part of our review. Looking for the tl;dr? Scroll to the end!

## Further detail pages

In the passage from the word search to the occurrences (see above!) the [lemma detail page](https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#lemma-detail-page) was already described. Also for the detail page of a sentence no further information is necessary. It corresponds to the view of the occurrences, has also the modification possibilities on the right side. In addition, the detailed view of the sentence has the citation note, which has already been [criticized in detail for the lemma detail page](https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#Citation-note). Finally, the page shows to which text this sentence belongs and the persistent IDs. In the following the further detail sides are presented.

### Text

You can get to the detail page of a text either directly by entering the ID on the search page or by clicking on the link from a sentence that belongs to this text. After the heading with the text name and ID, the persistent ID and the persistent URL can be found at the top. Only then the metadata follow.

The representations of the metadata in the old TLA, in ORAEC and in the new TLA are compared here. The medical text on [pBM EA 10059](https://www.trismegistos.org/text/380900) is selected as an example.

---

#### Metadata in the old TLA

![10059 in the old TLA](/img/tla_review/10059_old.jpg "10059 in the old TLA")

#### Metadata in ORAEC

![10059 in ORAEC](/img/tla_review/10059_oraec.jpg "10059 in ORAEC")

#### Metadata in the new TLA

![10059 in the new TLA](/img/tla_review/10059_new.jpg "10059 in the new TLA")

---

The old TLA has six metadata fields here: bibliography, line count according to, provenance, date, type of object, and script. It is curious that the object-related metadata is listed. ORAEC, which brings together text and object metadata, has seven metadata fields: textname, date, findspot, object, location, inv. no., and bibliography. Here line count according to and script are missing. Instead, the object-related fields location and inv. no. have been added. The new TLA offers seven metadata fields data type, dating, script, language, finding place, current location and bibliography. Data type describes the type of database object, i.e. here: text. Only the new TLA offers the field language, which at first sight is a welcome innovation. In reality, such a label is ill-suited to describe Egyptian texts from the middle of the second millennium onwards. This is because they often have several language strata that are used together and simultaneously in the text. It is not very useful to try to express the diversity of a text with a single label. Instead, one would have to assign individual passages to the respective language strata. When everything has the same label "Égyptien de tradition", it no longer has any informational value. In this respect, this innovation is rather misleading. Also like the old TLA, the new TLA offers some object-related metadata. But unlike the old TLA, the text-bearing object does not have this metadata in the new TLA! Finding place and current location only exist in the metadata of the text, but not of the object! This has gone wrong in the conception of the representation of the metadata!

After the bibliographic information there is a nice new feature. The external references provide links to other projects that also deal with this text. Thus, there are references to [Ramsès](http://ramses.ulg.ac.be/). Apparently, the new TLA can also access material by Ramsès that has not yet been published. For example, at <https://thesaurus-linguae-aegyptiae.de/text/VSII7CW7F5GS7HA6VOGKZSY4BA> a link is given that leads to a [page in Ramsès](http://ramses.ulg.ac.be/text/legacy/846) that says: "This text does not exist, or is not published online yet." The ID of the inscriptions of the early period (cf. [Sperveslage, Gunnar: Die frühen Inschriften Ägyptens. A concordance of numbering systems. 2021](https://aegyptiaca.uni-muenster.de/Record/122784)) is given but not linked. ![inscriptions of the early period](/img/tla_review/PBFK5R4STJA3RN2BTSXSMABF5M.jpg "inscriptions of the early period") Unfortunately, there is no link to the old TLA. This is a pity. Probably the effort to do a mapping is too big. But in many cases a link could have been generated computer aided, and this if the object is linked to Trismegistos. Here is an example: the [demotic text Heidelberg 785](https://thesaurus-linguae-aegyptiae.de/text/PTZSWPXJDFGMVHLT4RQVZVAAU4) is written on the [object Heidelberg 785](https://thesaurus-linguae-aegyptiae.de/object/GEJBNQXJXFATVO6EN664PLHFHY). On the detailed view of the object there is a link to [Trismegistos](https://www.trismegistos.org/text/55961). ![Trismegistos text 55961](/img/tla_review/55961.jpg "Trismegistos text 55961") There is a link to the [text in the old TLA](https://aaew.bbaw.de/tla/servlet/OTPassport?db=1&oc=77). So all you have to do is collect the links from Trismegistos and append them to the corresponding text in the new TLA to generate a link in the old TLA.

As with the occurrences, a path is specified here. For the path see [above](https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#path)!

The next section presents the elements of the hierarchy that are either directly superordinate to the text or directly subordinate to the text. Note that the mentioned elements are not sorted. Unfortunately, the sentences subordinate to the text are not displayed. That is, you cannot look at the text in transcription and translation. Only the metadata remains. This shortcoming will surely be fixed soon.

As in the lemmadetails page there is now a field with main author, further editors and the time of the last change. For this see [above](https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#author)! There is also as fourth the redaction status. This means that there is a possibility that the new TLA can offer not only obsolete lemmas, but also obsolete texts. One can be curious with which sense such information will be filled!

Finally, there is the citation note, which has already been criticized in detail [above](https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#citation-note). One can only hope that the many [collaboration partners](https://thesaurus-linguae-aegyptiae.de/info/authors) who have supplied texts to the new TLA are not now annoyed that they, who have done all the work, are not mentioned in the notice.

### Object

The detail view of the object is built in the same way as the detail view of a text. Note, however, that the name of the object does not appear in the ``title`` of the ``head`` of the HTML document. As noted above, the object-related metadata finding place and current location are missing. True, the new TLA promises, "(More metadata in a future version of the TLA web app.)". But there is the assumption that these metadata were deliberately omitted here, because they are given with the text. Here the conception should be urgently improved.

As with the text, there is the field external references. Also here this field is to be praised very much! There are links to the [British Museum](https://www.britishmuseum.org/collection) and to [Trismegistos](https://www.trismegistos.org)

As with the text, the ID from the inscriptions of the early period is given, but not linked. [In one case](https://thesaurus-linguae-aegyptiae.de/object/RS2BRP2CSJACPMYVIPE2YWFPDI) we also found a link to the [Museo Egizio](https://museoegizio.it/en/), but it leads to password protected content: <http://papyri.museoegizio.it/o/161>.

### Thesaurus

The new TLA offers detail views also for thesaurus entries. If we see it correctly, these entries can be accessed by link only via the detail view of a sentence. Another way to access these entries is by entering the ID. One can get the IDs directly from [thesaurus.xml of the AED-TEI](https://github.com/simondschweitzer/aed-tei/blob/master/files/thesaurus.xml) or obtain them from the [partial extract](https://nbn-resolving.org/urn:nbn:de:kobv:b4-opus4-29190).

Again, there is the wonderful external references field. Listed here are [GND](https://en.wikipedia.org/w/index.php?title=Integrated_Authority_File&oldid=1102094625), [Multilingual Egyptological Thesaurus](https://aegyptiaca.uni-muenster.de/Record/12843) hosted by [Projet Rosette](https://projetrosette.info/page.php?Id=1), [Thot](https://thot.philo.ulg.ac.be/), [Topographical Bibliography](http://topbib.griffith.ox.ac.uk//index.html), [Trismegistos](https://www.trismegistos.org), and [Wikidata](https://en.wikipedia.org/w/index.php?title=Wikidata&oldid=1122235823).

The links to Trismegistos are unfortunately wrong. For example, the entry for the place [Hazor](https://thesaurus-linguae-aegyptiae.de/thesaurus/QF6KKTLEMVCALOZRON4JAI5IGM) links to <https://www.trismegistos.org/text/50861>. ![Trismegistos text 50861](/img/tla_review/50861_text.jpg "Trismegistos text 50861") But what is meant is <https://www.trismegistos.org/place/50861>! ![Trismegistos place 50861](/img/tla_review/50861_place.jpg "Trismegistos place 50861")

The links to the project [Aegaron](http://drupaldev.aegaron.ucla.edu/) are not displayed correctly: ![Aegaron](/img/tla_review/FEO6RBKYTBCYNHD4IWIVAZI7V4.jpg "Aegaron").

There is also a reference to an entry of the old TLA. However, this is done without a link. Is this perhaps an internal note? Anyway, the Linked Data section of the thesaurus entries is excellent. This is - somewhat surprisingly - one of the best features in the new TLA! Many thanks.

We want to highlight one detailed view: <https://thesaurus-linguae-aegyptiae.de/thesaurus/OJDRAHAIX5BMND7OQH3TKTG4C4>. There are a lot of Egyptologists listed here. Does the new TLA have, say, a bibliographic database in the background?

## Data

The previous description of the new TLA focused on the interface: how to get to the information you are looking for and how to display it. The following is about the data itself.

### Raw data

The data itself can only be accessed via the web interface. You either have to submit a search or go directly to an ID. For the above description of the thesaurus entries, this was exceedingly tedious. Unfortunately, the raw data has not yet been published. We hope that the [promise](https://thesaurus-linguae-aegyptiae.de/info/licenses) "You will find a link to the citable and reusable raw data soon on the web page" will be kept soon. One web page cannot provide all searches. That's why there must be free data, so that everyone can do independent research with it! In our ORAEC project we plan to show some visualizations. This is only possible with free data!

### Quantity

According to its own statement, the new TLA has "1.44 mill. lemma tokens". If we had raw data, we could verify that. Also, the number of word forms in the old TLA is not entirely clear. [The introductory text in the old TLA](https://aaew.bbaw.de/tla/servlet/S05?d=d001&h=h001) speaks of "1,400,000 text words." [A report on the text encoding software of the Thesaurus Linguae Aegyptiae](https://nbn-resolving.org/urn:nbn:de:bsz:15-qucosa-201766) claims it is "1.2 million text words". If we understand the statement about Edfu project data in the [development plan](https://thesaurus-linguae-aegyptiae.de/info/tla-development) correctly, the Edfu project data are not included in the new TLA. This means that the increase in data from the old to the new TLA can be estimated at around 300,000 tokens (with some [magical multiplication of occurrences](https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#magical-multiplication-of-the-occurrences)). External collaborators are responsible for a not small part, e.g. the project on the early period in Cologne or the project on the grammar of the 18th dynasty. Considering that there are eight years between the publication of the old and the new TLA, it must be stated that the main focus of the work at the Berlin-Brandenburg Academy of Sciences and Humanities and Saxon Academy of Sciences and Humanities in Leipzig has not been in the area of corpus building.

### Quality

Joachim Friedrich Quack addressed the data quality of our ORAEC corpus in an email to the EEF mailing list on October 30, 2022. The ORAEC data come from [AED](https://simondschweitzer.github.io/aed/) and [AES](https://github.com/simondschweitzer/aes), which in turn are based on the [partial extract of data from the TLA](https://nbn-resolving.org/urn:nbn:de:kobv:b4-opus4-29190). Thus, Quack's critique is also a critique of the TLA's data quality. He is specifically concerned with the text [oraec2](https://oraec.github.io/corpus/oraec2.html), which can be found in the new TLA at <https://thesaurus-linguae-aegyptiae.de/text/L7D5AZI5SRBY7KDHPSKJURRZK4>. Quack's first criticism is that there are now new fragments of this text that he [published](https://aegyptiaca.uni-muenster.de/Record/124435) last year, but they were not included. This is difficult to check for the new TLA, since neither the raw data are published nor the text is shown in transcription. However, the bibliography for this text is at the same level as for the partial excerpt, and the sentences of the text have received virtually no revision. Thus, it can be assumed that the new fragments have not been incorporated in the new TLA either. Second, Quack criticizes the fact that in two places in the text Ḥw-mḥn is incorrectly transcribed instead of the correct Ḥrn for the god Hauron. In the old TLA there is a separate [entry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?wn=856431&db=0) for Ḥw-mḥn. The two occurrences from the text oraec2 are also filed there. Between 2014 and 2018, this entry was locked and the occurrences were redirected to the correct lemma Ḥrn. This is the finding from the partial excerpt: The lemma there has the redaction status "published-obsolete". The occurrences from oraec2 are associated with the correct lemma Ḥrn. This is exactly how it appears in ORAEC. The two tokens referred to by Quack are oraec2-170-7 and oraec2-177-2. As can be clearly seen in the sentence representations <https://oraec.github.io/corpus/oraec2-170.html> and <https://oraec.github.io/corpus/oraec2-177.html>, the two tokens are associated with the correct lemma Ḥrn. ![oraec2-170](/img/tla_review/oraec2-170.jpg "oraec2-170") ![oraec2-177](/img/tla_review/oraec2-177.jpg "oraec2-177") The data finding in the new TLA is identical to that of ORAEC. The lemma [Ḥw-mḥn](https://thesaurus-linguae-aegyptiae.de/lemma/856431) is obsolete, which is not made directly clear by the designation "inactive". In both sentences <https://thesaurus-linguae-aegyptiae.de/sentence/IBUBd3L5zOOP4UhPgxYBNISG4cA> and <https://thesaurus-linguae-aegyptiae.de/sentence/IBUBdzy60bdUek4vgc9h6r5MNPM>, Ḥw-mḥn is transcribed but lemmatized as [Ḥrn](https://thesaurus-linguae-aegyptiae.de/lemma/109070). ![first occurrence](/img/tla_review/IBUBd3L5zOOP4UhPgxYBNISG4cA.jpg "first occurrence") ![second occurrence](/img/tla_review/IBUBdzy60bdUek4vgc9h6r5MNPM.jpg "second occurrence") Unlike ORAEC, however, the lemma is not explicitly noted with the sentence, so a user cannot directly see the lemma a word form is lemmatized with. The criticized data are identical in ORAEC and in the new TLA. One might now think that Quack's final verdict "To me, it seems that some more deep-seated re-working is needed if this site wants to be a really useful instrument." thus also applies to the new TLA. We don't want to gloss over the quality problem, but we do want to point out another aspect. In large projects, a lot of data accumulates over time. How can you guarantee that the data can always be revised? This revision is a weighty time factor. The more data, the more time is actually needed. The only thing is that revising does not do justice to the scientific reality. Applications that mainly want to revise data will not be approved. In the current situation of science funding, it is simply not possible to keep all inherited data completely up-to-date at all times. Probably a larger discussion is needed in the Egyptological community on how to deal with this problem. We propose to use ORAEC and the new TLA, even if parts of the data do not represent the latest knowledge. Errors occur in all data, including digital data. The researcher has an obligation to always handle them carefully and critically.

Another aspect of data quality in the new TLA is more about project management; because the data are the real treasure of the new TLA. The data quality is appropriate of a large project used by many Egyptologists. However, it is evident that too little emphasis is placed on correction phases in the new TLA. Take as an example the occurrences for the [dog name Nb](https://tla.bbaw.de/search/sentence?tokens[0].lemma.id=879977). Four of the five occurrences are the adjective nb. There is simply a lack of quality control.

## Next steps

The new TLA provides a [comparison between old and new TLA](https://tla.bbaw.de/info/tla-development). The purpose of this overview is clear: the new TLA is to be presented as a big step forward compared to the old TLA. However, quite a few details of the old TLA are simply wrong, so that one can wonder whether the new TLA was deliberately intended to be better or whether the creator of the table is unaware of many features of the old TLA. Here are a few of the errors from this overview:
* "Lemmata: attestation time span in the TLA corpus" Of course, one can easily find out the attestation time span in the old TLA. Unlike the new TLA, the attestations are sorted there. The attestation time span is simply the span from the first to the last attestation, which can be read quickly.
* "Lemmata: English, French translation equivalents" The overview claims that all lemmas have English translations: "EN: completed, FR: partly". This is impertinent; for not a single demotic lemma has an English translation.
* "Lemmata: linking composites/parts (ḥm-nṯr > ḥm, ...)" Of course, this feature already exists in the old TLA. The demotic list makes extensive use of it. Does the creator of this overview not know the demotic list, or is the demotic not that important to him?
* "Sentence words: hieroglyphs" The overview represents it in such a way that now all words would have hieroglyphs. This is not the case. Just like in the old TLA, many texts lack hieroglyphs.
* "Sentence words: contextual meaning" Of course, the old TLA offers the contextual translation of a word. ![contextual translation in the old TLA](/img/tla_review/cotext_translation_old.jpg "contextual translation in the old TLA") It can be found in the header of an occurrence.
* "References to other digital projects" Of course, there are already references to other projects in the old TLA, for example in the demotic list for [DWL](https://www.dwl.aegyptologie.uni-muenchen.de/).

These errors alone make the page a nuisance. But it is even worse: This is actually a development plan. The prioritization is already strange. Who really thinks a feedback form is more important than sorting the hit list and occurrences? But the plan reveals a lot about what is not thought of at all: a search for the grammatical annotations, for example, is not planned at all, a search for the thesaurus entries is not mentioned either. One really gets the impression that the management of the project has no vision and does not know what to do with the treasure trove of data. This is scary.

## Conclusion

Let's summarize. The design is fresh. The technical foundation is excellent. The data material is a treasure, as we can all see by the fact that the words are not only transcribed, translated and lemmatized, but also grammatically annotated. And of course, because of the cool data, the new TLA has great things that you can just praise. But the implementation is not satisfactory. The problems are twofold:

### Not yet

However, the new TLA does not yet have the functionality of the old TLA. It says so quite openly. Why use it if it doesn't yet provide appropriate tools to mine the great treasure trove of data? So, because of the new words and because of the new texts? After all, the texts are not displayed at all, and the search for words and the display of the occurrences frustrate the user because of the lack of sorting. Nevertheless, we recommend the use of the new TLA for very specific use cases:

* The new TLA is worthwhile for anyone interested in the early period. The new TLA now has a lot of language data from this era. One [searches in the bibliography field](https://thesaurus-linguae-aegyptiae.de/search/lemma?script=hieratic&_script=on&_script=on&transcription.text=&transcription.enc=unicode&wordClass.type=&root=&translation.text=&translation.lang=de&bibliography=Fr%C3%BCh%C3%A4gypt) for "Frühägypt" for Kahl, Jochem: Frühägyptisches Wörterbuch, 2002-2004.

* One can find words in a joint search in the Egyptian and Demotic lists.

* The data, especially the thesaurus entries provide quite a lot of Linked Data.

For all other use cases we recommend to use another product, e.g. [AED](https://simondschweitzer.github.io/aed/), [DPDP](https://demotischdemotisch.de), [ORAEC](https://oraec.github.io/corpus/), but especially the old TLA!

### Strategy

More serious are the strategic errors made by the project management, which we encountered repeatedly in writing this review. One gets the impression that the management does not really know the contents of the data at all, which explains the problems in the designations described many times above, and that the management lacks a vision of what it should actually do with the data. The new TLA is also not able to combine the different data - highly structured thesaurus entries, reusable linked data on the one hand, unstructured lemma annotations on the other hand - into a homogeneous synthesis. This is a great pity! Because the world cup is about to start, a comparison from soccer is allowed: Design, technical infrastructure and the data have put the ball right in front of the empty goal, yet the shot misses with the new TLA.

## tl;dr

The new TLA has a fresh design, excellent technical infrastructure and great data. The implementation, however, disappoints, making it frustrating to use. Let's wait for an update! Otherwise, the following applies: If you want to find something specifically, you should go back to the [old TLA](https://aaew.bbaw.de/tla/index.html) or (for the demotic data) use [DPDP](https://demotischdemotisch.de)!