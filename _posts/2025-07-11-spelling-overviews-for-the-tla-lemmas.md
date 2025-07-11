# Spelling overviews for the TLA lemmas

Hi, guys! It's been a long time since our last post. We're still busy working on a large body of text. But here's a sign of life from us!

As you know, the [TLA](https://thesaurus-linguae-aegyptiae.de/) has an incredibly rich collection of texts with many hieroglyphic spellings. The first version of the new TLA included almost 700,000 word forms with hieroglyphic spellings. It was not possible to search for these spellings in the TLA. Therefore, we made these spellings accessible via [our metasearch engine](https://oraec.github.io/corpus/search/). The current version has nearly 950,000 word forms annotated with hieroglyphs. At the same time, the TLA has made an overview of spellings per entry available.

![Spelling TLA Overview](/img/blog/spelling_tla_overview_mrt.jpg "Spelling TLA Overview")

The hieroglyphs are encoded in Unicode, and the grammar of each word form is provided. There are also links to the references. Cool, isn't it? This is the TLA's first step to making its rich treasures accessible, but, to be honest, it's only a small one. There are several points of criticism that we would like to illustrate using the example of the lemma ꜣḫ "akh spirit" (ID 203).

## Sorting

There are many ways to write our example. This raises the question of how the material should be sorted. The TLA has decided to sort it alphabetically according to the Gardiner codes of the hieroglyphs. The corresponding Gardiner codes are G1-G43-Aa1-G25-G25-G25, G25, and G25-A1, resulting in the sequence 𓄿𓅱𓐍𓅜𓅜𓅜𓅜, 𓅜, and 𓅜𓀀. The advantage is that the sorting is clear and comprehensible. However, the disadvantage is that the user can't easily see how a word is usually spelled because this alphabetical sorting places unusual and high-frequency spellings next to each other. It would be more user-friendly to sort by frequency.

## Morphological annotation

The TLA categorizes spelling occurrences based on grammatical annotation. For example, occurrences of 𓅜𓐍 fall into three categories: cases with no grammatical annotation, singular cases, and singular cases of the status pronominalis. However, this distinction seems trivial when it is specifically indicated that spellings with 𓏥 are plural. Of course, inflection influences spelling. Nevertheless, we believe that factors such as the script and date are more influential on spelling than grammatical annotation. Hieroglyphic monumental inscriptions and hieratic papyri often have different spellings for the same word, as one quickly realizes when reading Egyptian texts. The date of a text has an immense influence on its spelling. In our example, the hieroglyph 𓇶 was only used from the Late Period onwards. Sorting the spellings by chronological location reveals this information quickly. Unfortunately, the current TLA sorting does not reveal this information.

## Non-unique list entries

In our example, there are so many spellings that it is difficult to keep track of them all. The TLA exacerbates this issue by duplicating some entries. For example, 𓅜𓐍𓏲𓀼𓏥 and 𓅜𓐍𓏲𓀽𓏥 appear twice; there are two identical spellings of each.

![Double entry 1](/img/blog/spelling_tla_same_spelling_1.jpg "Double entry 1")

![Double entry 2](/img/blog/spelling_tla_same_spelling_2.jpg "Double entry 2")

Furthermore, our [recommendations for encoding Egyptian hieroglyphs in Unicode](https://oraec.github.io/2022/09/28/recommendations-encoding-hieroglyphs.html) are not taken into account. This has the major disadvantage that <https://thesaurus-linguae-aegyptiae.de/sentence/token/IBUBd11L0EWD1Eynjk2PVHcxAws> is not listed with the other occurrences for 𓅜𓐍𓀭𓏥, simply because the phonogram 𓅜 has a paleographic variation that cannot be located at the sign variance level.

## Quantity of Occurrences:

If a spelling has more than 11 occurrences, only 11 occurrences are linked. Therefore, the TLA does not allow for the examination of high-frequency spellings.


Due to these criticisms, we decided to compile our own spelling overview to reveal the treasures of the TLA. We have created a separate spelling chart for each TLA entry with hieroglyphic spellings. The overview begins with a list of all spellings of a word, sorted by frequency, and indicates how many times each spelling occurs. This is followed by a chronological distribution of spellings. First are the spellings from the Pre/Early Dynastic Period, followed by those from the Old Kingdom, the First Intermediate Period, and so on, up to the spellings from the Greco-Roman Period. Lastly, we list the spellings for which the TLA does not provide a date. Within each period, spellings are organized by script. Spellings written in hieroglyphs are listed first, followed by spellings written in hieratic. The spellings are sorted by frequency, allowing the meaning of a spelling to be quickly assessed. In each spelling category, there are links to occurrences in the TLA. Each link contains the name of the text, allowing you to quickly determine the relevance of a specific occurrence.

![Spelling Overview ORAEC](/img/blog/spelling_tla_oraec_203.jpg "Spelling Overview ORAEC")

How do you access these spelling overviews? There are three different ways:

## 1) Address bar

The web pages are all located in the repository <https://github.com/oraec/tla-spelling-overview>. If you know the ID of a lemma, you can go directly to the spelling overview of a lemma. In our example, the lemma has the ID 203, so the URL of the spelling overview is <https://oraec.github.io/tla-spelling-overview/203.html>. For any other lemma, you can simply enter the corresponding ID in the address bar instead of "203".

## 2) Chrome Extension

There is also a Chrome extension that can be accessed at <https://github.com/oraec/tla-spelling-overview-chrome-extension>. This add-on adds a link to every TLA web page of a lemma. This link called "Visit Spelling Overview" leads to our spelling overview.

![Chrome Extension](/img/blog/spelling_tla_chrome_extension.jpg "Chrome Extension")

## 3) Metasearch Engine:

As you know, our metasearch engine searches hieroglyphic spellings in various projects, including AED, ORAEC, PNM, Prosopographia Aegypti, Ramsès, STaTbS21D, and Wikisource. The TLA can also be accessed through our search engine. We have updated our search engine. The search now leads directly to our writing overviews. This update has several advantages. First, the search now includes the current TLA data set, which contains almost 40% more hieroglyphic spellings than the one used previously. The search is faster because not all token IDs are reloaded in the search engine. Spelling overviews now provide text names, whereas the previous metasearch only provided occurrence numbers. Finally, the link from the spelling overview now leads directly to the highlighted word form, rather than just to the sentence as before.

No matter how you use it, we hope the spelling overviews help you make the TLA more accessible.

See you next time! It will probably take a while because the text corpus we're working on is quite large.

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a></p>
