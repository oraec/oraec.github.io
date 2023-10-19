# Text display in the new TLA

## Finally! Text display in the new TLA

Hi folks! Since last weekend the new TLA has a new and important feature: Finally the texts are offered in transliteration and translation! Congratulations to the project! And welcome to the world of corpus linguistic projects! Therefore, this blog is dedicated to this new feature and the developments of the new TLA during the last year.

Unfortunately, there is no text search. Instead, you can access the new pages in two ways. On the previous text page, there is a button to view the entire text. Second, there is a button to view the full text of a sentence you may find at the occurrences.

![Textview](/img/tla_review/textview.jpg "textview")

This is how the view of a text looks in the new TLA. The new TLA separates the view into two different pages, one with only the metadata and one with only the actual text. In the example shown, these are the pages <https://thesaurus-linguae-aegyptiae.de/text/AN4EQTJBRBBB5JJXDFRMBTPFEM> and <https://thesaurus-linguae-aegyptiae.de/text/AN4EQTJBRBBB5JJXDFRMBTPFEM/sentences>. The structure is easy to see from the address. You get to the general data for the text by specifying its ID. For the text itself, add "/sentences" to the address. This distinguishes the new TLA from the old TLA, which has sentences and metadata on one page. Instead, the new TLA follows our ORAEC pages, since we also distinguish between the text page and its edition page. We wonder if we inspired the new TLA?

For your comparison:

| Project  | Links to the text "Opferformel / Architrav des Ni-Ptah" |
| ------------- | ------------- |
| old TLA      | <https://aaew.bbaw.de/tla/servlet/GetTextDetails?u=guest&f=0&l=0&db=0&tc=10238> (metadata & edition)     |
| new TLA      | <https://thesaurus-linguae-aegyptiae.de/text/AN4EQTJBRBBB5JJXDFRMBTPFEM> (metadata)<br /><https://thesaurus-linguae-aegyptiae.de/text/AN4EQTJBRBBB5JJXDFRMBTPFEM/sentences> (edition)     |
| ORAEC      | <https://oraec.github.io/corpus/oraec5726.html> (metadata)<br /><https://oraec.github.io/corpus/oraec5726_text.html> (edition)     |

Like us, the heading only says the ID of the text, not the name of the text. The user has to look up AN4EQTJBRBB5JJXDFRMBTPFEM or oraec5726 on the metadata page. The text itself is divided into sentences. These sentences are separate rows in a large table that has four columns in the default view. The first column is the sequence number. So you can see how many sentences there are in the text. This is also reminiscent of the representation of sentences in ORAEC: oraec5726-2 is the second sentence of the text oraec5726. In the new TLA, the sequence numbers are links to the sentence view. The second column shows the hieroglyphs of the text. If the hieroglyphs are automatically arranged, the sentence gets the label "Glyphs artificially arranged" - as in the sentence view. This seems a bit redundant if all hieroglyphs of a text are automatically arranged. If there are no hieroglyphs, the default view will show this column anyway. I.e. all demotic texts have this empty column!

![Textview_demotic](/img/tla_review/textview_demotic.jpg "textview: demotic text")

The third column shows the transliteration of the sentence. As usual, the individual word forms are clickable and lead to the detailed view of the corresponding lemma. Unfortunately, all commas separating lexically relevant endings in the old TLA have been converted to dots. We criticized this at the time. Unfortunately, this problem occurs not only in the sentence view, but now also in the text view. Too bad! At the end of the transcription of the sentence there is sometimes a "With commentary". This corresponds to the "C" of the old TLA, when the editors have written comments on individual sentences. The fourth column contains the translation of the sentence.

On the right side there are several buttons. You can use them to show or hide the hieroglyphs and the translation. However, the first and the third column always remain. So if you want to copy the entire transliteration of a text, you will also copy the sequence number, the label "With commentary" and the label of the language of the translations. As in the sentence view, you can also turn on grammatical annotation. Great feature! Thanks a lot!

If the text consists of more than 10 sentences, the text is divided into sections of 10 sentences each. The pagination is at the top of the page. Finally, there is the path, the dating, the authors, the link to the metadata, and the citation.

Looks nice, doesn't it? Now comes the big drawback. The view is optimized for desktop only. On mobile it looks like this:

![Textview_responsive](/img/tla_review/textview_responsive.jpg "responsive textview")

Still, this is a great thing that the new TLA finally offers! Thank you very much! Let's take a look at what else has happened in the past year. Our review from last year will serve as a checklist. We'll list each of the criticisms mentioned there and see what progress has been made. Let's go!

## Checklist

### Comparison to the old TLA

> The new TLA is nowhere near the functionality of the old TLA, so it makes a lot of sense that the old one is not shut down. There is no combination search, no texts are displayed, the DZA is not integrated. (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#introduction>)

Now there is a combination search. Hooray! You have to enter the IDs of two words in the central search page. The concept of the search is the same as in ORAEC: A combination exists if the two words occur in the same sentence. The old TLA had a cross-sentence search instead. We wonder if the new TLA was inspired by ORAEC. The difference with us is that we offer more of an evaluation of collocations with related evidence, while the new TLA does not evaluate and summarize the data, but only offers a search. In other words, if you want to look up the collocation of zmy.t with the person name Jtj=sn in the TLA, you will get the occurrences: <https://thesaurus-linguae-aegyptiae.de/search/sentence?tokens%5B0%5D.lemma.id=134780&tokens%5B1%5D.lemma.id=710604> Those occurrences can also be found in ours, see <https://oraec.github.io/corpus/collocation_134780.html#aed_id710604>. Furthermore, <https://oraec.github.io/corpus/collocation_134780.html> provides an overview of all collocations of zmy.t, including an evaluation according to word types.

The text display has been available since last weekend, as explained above. Hooray! The DZA is still an external resource.

### Search

Search on the smartphone now doesn't have as much empty space as [before](https://oraec.github.io/img/tla_review/search_responsive.jpg):

![search_responsive_2023](/img/tla_review/search_responsive_2023.jpg "search responsive")

Thanks!

#### Transliteration

> Instead of the Egyptian yod, which exists since 2019 with [Unicode 12](https://unicode.org/versions/Unicode12.0.0/), a workaround is used. (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#transliteration>)

It still applies.

> Back to the Egyptian keyboard: An ï is offered, but the character is apparently not used in the word list at all. Why does one offer something for input that is not used at all? After all, no uniform font is used for the display. The ṱ comes from a sans-serif font, the t from one with serifs. Some characters like i̯, u̯ and h̭ appear corrupt. (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#transliteration>)

The ï does not make sense for the TLA, but it is in accordance with the recommendations of the [Leiden Unified Transliteration](https://oraec.github.io/2023/08/24/leiden-unified-transliteration.html).

![Keyboard_2023](/img/tla_review/keyboard_2023.jpg "keyboard 2023")

The font problem is solved!

> The second input method is called [Manuel de Codage](https://en.wikipedia.org/w/index.php?title=Manuel_de_Codage&oldid=1012543887), but it is not! For example, in the new TLA, ``i`` does not stand for ``j``, i.e. the character for 𓇋, but for ``i̯``. (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#transliteration>)

It still applies.

#### Regex

Unfortunately, there are no improvements at all. In detail:

> If you type ``_nn`` to find the demotic bird name \_nn, you get [28 results](https://thesaurus-linguae-aegyptiae.de/search/lemma?_script=on&script=demotic&_script=on&transcription.text=_nn&transcription.enc=unicode&wordClass.type=excl_names&root=&translation.text=&translation.lang=de&bibliography=). At the very end is the desired word. The superfluous use of ``_`` as a regex leads to poor precision. (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#transliteration>)

It still applies.

> Even the common words with parentheses, such as [jri̯ (ḫft.j)](https://thesaurus-linguae-aegyptiae.de/lemma/29220), cannot be found directly. Why annoy users by introducing nonsensical regex? (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#transliteration>)

It still applies.

> Also, the regex in the new TLA are buggy: a ``>`` is supposed to allow left truncation. A ``>-jmn`` leads to no result. You have to type ``>jmn`` instead. (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#transliteration>)

It still applies.

> Furthermore, regex are uncommon in general search engines. Or do you enter such characters in your Google search or your Amazon search? Instead, you use auto complete. Completions are suggested when you start typing. (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#transliteration>)

There is no auto complete.

> Furthermore a fuzzy search is also useful. Searches in the (old and now also in the new) TLA very often lead to zero results. The TLA distinguishes between ``s`` and ``z``. Your search for sꜣ, "son" leads to zero results because the entry in the TLA is zꜣ. The sun god is named Rꜥw, not Rꜥ. Horus is called Ḥr.w, not Ḥrw or Ḥr. The house is called pr, not pr.w or prw. How would anyone know? How will a casual user find anything here? Even the regex won't help you if you don't even expect that sꜣ won't bring the expected result. The search with the transcription is thus worse in the new TLA than in the old TLA. (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#transliteration>)

It still applies.

#### Word class

Originally, this field was called "Part of Speech", while elsewhere it was called " word class".

> In the next field, the word class is specified. Here it is *word class* as in the hit list and not *part of speech* as on the search page. (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#word-class>)

Now everything is unified. The selection of word types looks like this today:

![word_class_2023](/img/tla_review/word_class_2023.jpg "word class 2023")

Two entries have been added. While "(undefined)" is a useful addition, " Punctuation marks" is complete nonsense. This is a category error. A punctuation mark is not a part of speech, of course, because it is not a word. A search for this word type will return 0 hits in the new TLA. Why is this option there? Someone may have accidentally added this entry when editing the drop-down list without checking the edit. We have criticized the project management several times in the past year, and we can do so again on this point.

> Again, a misleading designation must be pointed out. While the English surface correctly speaks of “royal names”, in German it is called “Königs-/Königinnennamen”. [...] The names of the queens can be found in the old and new TLA accordingly with the personal names. (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#part-of-speech>)

This is corrected by adding "(regierende)".

#### Root

> Roots are treated there on the same level as normal words. If you search for nfr, you get regular words with the transcription nfr as well as the root nfr. (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#root>)

It still applies.

> If you enter nfr in the root field, you don’t get the root nfr, but all lemmas that belong to a root nfr. (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#root>)

It still applies.

> Finally, another oddity: In the root field, one can only enter Unicode, but no Manuel de Codage. Nevertheless, the radio button Unicode appears, to which one cannot make any changes. (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#root>)

It still applies.

#### Translation

> In contrast to the old TLA, you cannot use a regex here. A search for ``Bauc?h?`` leads to zero hits. (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#translation>)

It still applies.

> A search for ``bau`` also returns bauen, Baum, or Bauteil. The new TLA uses Elasticsearch search engine technology. Apparently, the search term is reduced to a base form. Searching for ``matte`` (mat) in the [new TLA](https://thesaurus-linguae-aegyptiae.de/search/lemma?script=hieratic&_script=on&_script=on&transcription.text=&transcription.enc=unicode&wordClass.type=excl_names&root=&translation.text=matte&translation.lang=de&bibliography=) also returns ``matt werden`` (become weak) (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#translation>)

It still applies.

#### Bibliography

> The old TLA makes it possible to find all lemmas that can be found on a particular page of the Wörterbuch. A search for ``Wb 2, 343`` returns all lemmas found on page 343 of the second volume of the Wörterbuch. [...] However, if one searches the new TLA, only one result is found, but it is not found on this Wörterbuch page: [Mri̯=s-gr](https://thesaurus-linguae-aegyptiae.de/lemma/72150). The bibliographic field of this entry has the content " Wb 2, 104.19 - Wb 5, 180.8 - LGG III, 343 ". The page number 343 is obtained from the LGG entry. Obviously, there is no phrase search. But without a phrase search this field is quite useless! (<https://oraec.github.io/2022/11/14/review-of-the-new-tla-part-one.html#bibliography>)

It still applies.

### Hit list

> The transcription appears - not only here, but always in the new TLA - in a font with serifs, while everything else appears in a sans-serif font. The mixture of serifs and sans-serif font creates a jarring impression. (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#hit-list>)

It still applies.

> Unfortunately, our [recommendations](https://oraec.github.io/2022/09/28/recommendations-encoding-hieroglyphs.html) have not been taken note of. Variants are encoded as characters: <https://thesaurus-linguae-aegyptiae.de/lemma/850775> has as hieroglyph 𓇋𓌳𓄪𓐍𓐍𓂋𓁹𓊨𓀭𓏅𓊽𓂧𓅱 instead of a 𓇋𓌳𓄪𓐍𓐍𓂋𓁹𓊨𓀭𓏃𓊽𓂧𓅱. (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#hit-list>)

It still applies.

> If you copy the hieroglyph characters from the hitlist, you get: 𓄿𓈎𓎛𓅱T7S. On the details page of the lemma, there is a special tool “Copy Unicode” that copies 𓄿𓈎𓎛𓅱<g>T7S</g> to the clipboard. Shouldn’t you expect the result to be the same? (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#hit-list>)

It still applies.

> The term “inactive” is misleading. It refers to the obsolete entries. (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#hit-list>)

It still applies.

> Furthermore, the hit list in the new TLA is always flat. All entries are on the same hierarchical level one after the other. The old TLA, on the other hand, offers not only the links from obsolete lemmas to regular ones, but also the hierarchical linking of lemmas, e.g. for prepositions and for verbs. (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#hit-list>)

It still applies.

> In this form, the specification of a attestation time in the new TLA is simply nonsense, which has no place in reasonable lexicographic research. (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#hit-list>)

It still applies.

### Lemma Detail Page

> <https://thesaurus-linguae-aegyptiae.de/lemma/865595> has as hieroglyphic writing the already mentioned 𓍑𓄿𓏵𓄿𓈎𓂋𓏏𓉐𓏥. [...] According to Manuel de Codage, however, it should read U28-G1-Z10-G1-N29:D21-X1\*O1:Z2. Unicode only gives the order of the hieroglyphs, but not the arrangement. This becomes visible on the page by using a font that uses OpenType ligatures. This is a highly recommended solution to deal with the arrangements. However, in Manuel de Codage these arrangements are hard coded. Thus, the information differs depending on the encoding type, since Manuel de Codage includes the lexicographically redundant information of the arrangement. Furthermore, the arrangement of the characters does not match. Why is the visual impression different from the information Manuel de Codage offers? In this respect, the code according to Manuel de Codage is misleading, and this button copy MdC is more disturbing than useful. (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#lemma-detail-page>)

It still applies.

> The mapping between Unicode and Manuel de Codage is unfortunately not correct. In Unicode there is a ``¿``, while in the image a ``⸮`` is used, cf. <https://thesaurus-linguae-aegyptiae.de/lemma/700540>. (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#lemma-detail-page>)

It still applies.

> The abbreviations used are broken down in a separate page <https://thesaurus-linguae-aegyptiae.de/listings/bibliography> Unfortunately, this page is not always correct in alphabetical sorting. Furthermore, quite a few titles are missing there (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#lemma-detail-page>)

It still applies.

#### External references

> For the [Vocabulaire de l'Égyptien Ancien](http://vega-vocabulaire-egyptien-ancien.fr/) there is only the indication of the ID, but no link. (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#external-references>)

It still applies. ORAEC offers a direct link to the VÉgA entry, cf. <https://oraec.github.io/2023/07/25/oraec-and-vega.html>.

> It is somewhat strange that two very important digital projects on Egyptian lexicography are missing, namely [DPDP](https://demotischdemotisch.de) and [AED](https://simondschweitzer.github.io/aed/). (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#external-references>)

It still applies, but DPDP is listed in the [Digital References of the TLA](https://tlabeta.bbaw.de/listings/digital-references?lang=en).

#### Comment

> The reader is left perplexed when he reads, for example, the comment in <https://thesaurus-linguae-aegyptiae.de/lemma/854631>. [...] Is now to read mꜣš.t as the entry is set in the TLA, or mš.t as it is at the beginning of the paragraph in the comment? Is the referenced identification of the duck that Boessneck makes now the prevailing view? How is it to be evaluated? This is simply pouring out a box of notes without coming to a conclusive conclusion. (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#comment>)

It still applies.

> The commentaries appear within the new TLA as a foreign body that is not properly integrated. For example, Peter Dils writes in his comment for the Egyptian word for placenta <https://thesaurus-linguae-aegyptiae.de/lemma/880484>: "Bezeichnung der Plazenta", while he translates, however, in the two occurrences of the word "Mutter(kuchen)". (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#comment>)

It still applies.

> The comment to <https://thesaurus-linguae-aegyptiae.de/lemma/132250> mentions another plant name and references the Wörterbuch, but does not give the ID of the lemma from the TLA <https://thesaurus-linguae-aegyptiae.de/lemma/132240>! (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#comment>)

It still applies.

> Also, the interaction between the actual lemma entry and the comment does not work. <https://thesaurus-linguae-aegyptiae.de/lemma/872159> is set as tp.t-hdn, while Lutz Popko writes dp.t-hdn in his comment. Who reads after the convincing paper by [Roberson, Tête-à-tête. Some Observations and Counter-Arguments Regarding a Contentious Phonological Value, dp or tp. In: LingAeg 26, 2018, 185-202,](https://aegyptiaca.uni-muenster.de/Record/114621) still dp instead of tp? (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#comment>)

It still applies.

#### Author

> Also the difference between main author and further editors is not clear. (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#author>)

The terms have been improved. Now it is "editor(s)" and "with contributions by". This makes it easier to understand.

> Also the sorting of the further editors is not obvious. In <https://thesaurus-linguae-aegyptiae.de/lemma/855167> it says "Emilia Mammola, Simon D. Schweitzer", but in <https://thesaurus-linguae-aegyptiae.de/lemma/713892> it says "Simon D. Schweitzer, Emilia Mammola". Is the order due to the number or relevance of the changes? (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#author>)

It still applies.

> The time of the last change is given in the format MM/DD/YYYY. Why is [ISO 8601](https://en.wikipedia.org/w/index.php?title=ISO_8601&oldid=1118528600), the usual YYYY-MM-DD, not used? (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#author>)

It still applies. Sometimes, there is a "before June 2015 (1992–2015)". The parentheses are superfluous.

#### Citation note

> This license requires author attribution, but this citation neglects to do so. (<https://oraec.github.io/2022/11/15/review-of-the-new-tla-part-two.html#citation-note>)

Fortunately, this has been corrected.

### Occurrences

#### Hieroglyphic writing

> Sometimes only some sentences of a text have this clue (="Glyphs artificially arranged"), but others do not, cf. <https://thesaurus-linguae-aegyptiae.de/search/sentence?tokens[0].lemma.id=708574>. (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#hieroglyphic-writing>)

It still applies.

> Moreover, the same facts are treated differently: In <https://thesaurus-linguae-aegyptiae.de/sentence/IBUBd1VqSFbrdEXXkmGOCucFn58>, ``F1*Z3`` is coded first, and ``H1-Z3`` is coded immediately afterwards, although the same coding should be present in both cases; because the order animal head + plural strokes is present in both cases. (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#hieroglyphic-writing>)

It still applies.

> This [example](https://thesaurus-linguae-aegyptiae.de/sentence/IBUBd4UwAExhxk1FjTomHEaKOwg) also shows the big mess with destruction specifications. [...] A gap of 1.5 rectangular groups is represented in this sentence in three ways: either as a shade mark, or by square brackets with a 1.5Q between them, or by specifying about 1.5Q without square brackets. Some occurrences have a ``[...]``, some have a shade mark. However, in the data from the partial excerpt, only the ``//`` is documented as a shade mark. Why was disambiguation done? (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#hieroglyphic-writing>)

It still applies.

> Again, different standards are encountered: <https://thesaurus-linguae-aegyptiae.de/sentence/ICECgs7eOzWZWUvNsqWie4d3L8E> omits the encoding of hieroglyphs in haplography, and <https://tla.bbaw.de/sentence/IBUBd9tf5Ak190sOtbY4xeJsNn8> annotates haplography. (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#hieroglyphic-writing>)

It still applies.

> In addition, signs are annotated which seem to exist only in an internal character set. <https://thesaurus-linguae-aegyptiae.de/sentence/ICICh9L2FWXiPUjPq80eLndHxp0> has a ``US9I3VARA`` that could not be converted to hieroglyphics. [...] Such undocumented annotations are poison for long-term use of the data. In this form, the treatment of hieroglyphs in the text corpus is a huge step backwards compared to the old TLA! (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#hieroglyphic-writing>)

It still applies.

> Latin text is occasionally placed between the hieroglyphs, the meaning of which is not documented anywhere. <https://thesaurus-linguae-aegyptiae.de/sentence/IBUCkyan7yNEmUz9mIveSP9M0bs> has ``var`` and ``?var?``. The above mentioned sentence <https://thesaurus-linguae-aegyptiae.de/sentence/IBUBd4UwAExhxk1FjTomHEaKOwg> has an ``lb``. <https://thesaurus-linguae-aegyptiae.de/sentence/5FLJWXUSC5C4LHEZ3WNAYZTDPU> has a ``mono``. <https://thesaurus-linguae-aegyptiae.de/sentence/IBUBd0PdqTaKbkNsoTMaP9YJa1o> has ``hierat``. You can guess that ``lb`` stands for line break. (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#hieroglyphic-writing>)

Documentation is still missing.

> This kind of markup is more important in the data than the correct encoding of the characters. Thus, in <https://thesaurus-linguae-aegyptiae.de/sentence/IBUBdxOUYzUQYUVDjmZPjzsCXt8>, the ``lb`` is written in 𓈗. This splits the character 𓈗 into three 𓈖, incorrectly postulating a spelling of mw, "water" with three individual 𓈖! (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#hieroglyphic-writing>)

It still applies.

> Modern paragraph references are also placed between the hieroglyphs, but the line counts are missing, cf. <https://thesaurus-linguae-aegyptiae.de/sentence/IBUBd0LS7PQWpEfhutqMKzlSRPY>. (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#hieroglyphic-writing>)

It still applies.

> Verse points are also integrated into the hieroglyphic text, cf. <https://thesaurus-linguae-aegyptiae.de/sentence/IBUBd3Jqxbw1U0Q3kfziqhNFMsI>, [...] although the transposition as verse points is not always successful: <https://thesaurus-linguae-aegyptiae.de/sentence/IBUBd3bPaK7Fi0YLha3A2ingCos>. (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#hieroglyphic-writing>)

It still applies.

#### Transcription

> Rubra are underlined, which is somewhat illegible with the underscores and dots in the Egyptological transcription, cf. <https://thesaurus-linguae-aegyptiae.de/sentence/HTDDBK3QINA57CQ7O5PB526CTM>. (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#transcription>)

It still applies.

> First, the new TLA converts all commas into dots. In doing so, the commas are a most welcome source of information, because the commas separate lexically relevant endings, while the dots indicate lexically irrelevant endings. In other words, a comma-delimited ending will appear in the dictionary, while a dot-delimited ending will not. This is a nice reading aid - popular among students - if you can distinguish directly between nb,t (the lady) and nb.t (feminine form of the adjective nb). Why is the added value abolished? (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#transcription>)

It still applies.

> Further, the new TLA capitalizes plural endings and dual endings, which - according to the partial extract - are encoded in the data as .pl and .du. This is uncommon and also sometimes leads to strange results like a Ḏꜣꜣ-qr(r).tPL in <https://thesaurus-linguae-aegyptiae.de/sentence/IBUBd9eXbgxXA0zSsm6BUICKNrc>. Why is time spent on this? (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#transcription>)

It still applies.

> Verse points are also included in the transcription. Unfortunately, they are rendered with ``•``; because that is the bullet, which has quite different semantics than the verse point. Better would be the ``·``. (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#transcription>)

It still applies.

#### Path

> The fact that <https://thesaurus-linguae-aegyptiae.de/sentence/3MP2R42KI5G4JBG26TZTVO7GAE> has no path specification for the [occurrence for nṯr](https://thesaurus-linguae-aegyptiae.de/search/sentence?tokens[0].lemma.id=90260) is certainly a mistake. (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#path>)

It still applies.

#### Reading variants

> Note that this multiplies the occurrences. This is because both reading variants are listed as independent occurrences for the word nṯr, cf. <https://thesaurus-linguae-aegyptiae.de/search/sentence?tokens[0].lemma.id=90260>. (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#reading-variants>)

It still applies.

#### Dating

> Occasionally a dating is missing, for example <https://thesaurus-linguae-aegyptiae.de/sentence/IBUBd3jwxnz1YUpVkt5xuD8FgOg>, although the dating is present in the old TLA: <https://aaew.bbaw.de/tla/servlet/GetTextDetails?u=guest&f=0&l=0&tc=402&db=1>. (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#dating>)

It still applies.

#### Sorting

> The biggest shortcoming of the records is that they are not sorted in any way. Even occurrences from the same text can be found on completely different pages. This is a disaster for high-frequency words, especially since it takes a long time to scroll through the pages. (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#sorting>)

It still applies.

#### Magical multiplication of the occurrences

> Occasionally, completely destroyed word forms are lemmatized when context makes the addition unambiguous. But <https://thesaurus-linguae-aegyptiae.de/sentence/IBUBd2p7DCqgEk5rsIsZgnG6Mt4> is too much of a good thing! [...] Here the whole sentence is destroyed and completely completed - probably because of parallels. Not even in the translation is it marked that the text has been reconstructed. But these five lemmatized word forms are among the "1.44 mill. lemma tokens". (<https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#magical-multiplication-of-the-occurrences>)

It still applies.

### Text

#### Metadata

> But unlike the old TLA, the text-bearing object does not have this metadata in the new TLA! Finding place and current location only exist in the metadata of the text, but not of the object! (<https://oraec.github.io/2022/11/17/review-of-the-new-tla-part-four.html#text>)

The metadata is revised, completed and appears in the right place. Thank you very much!

### Thesaurus

> The links to Trismegistos are unfortunately wrong. For example, the entry for the place [Hazor](https://thesaurus-linguae-aegyptiae.de/thesaurus/QF6KKTLEMVCALOZRON4JAI5IGM) links to <https://www.trismegistos.org/text/50861>. [...] But what is meant is <https://www.trismegistos.org/place/50861>! (<https://oraec.github.io/2022/11/17/review-of-the-new-tla-part-four.html#thesaurus>)

Now, the Trismegistos links are correct.

> The links to the project [Aegaron](http://drupaldev.aegaron.ucla.edu/) are not displayed correctly (<https://oraec.github.io/2022/11/17/review-of-the-new-tla-part-four.html#thesaurus>)

Now, there is "Ancient Egyptian Architecture Online" + ID.

### Raw data

> Unfortunately, the raw data has not yet been published. (<https://oraec.github.io/2022/11/17/review-of-the-new-tla-part-four.html#raw-data>)

It still applies.

## tl;dr

Finally, you can see the annotated texts in the TLA. Hooray! This is a major innovation. So the new TLA is being developed. The only thing to note is that the pace of development is quite slow. But the biggest problem is that the new TLA often produces the [error 502](https://www.howtogeek.com/356389/what-is-a-502-bad-gateway-error-and-how-can-i-fix-it/), so the TLA takes a long time to load, but you still can't access many pages. Dear TLA developers! Thank you for releasing the text view. But now please pay attention to the performance of the new TLA!

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a></p>
