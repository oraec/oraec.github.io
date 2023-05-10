# Metasearch engine for Egyptian hieroglyphs

## Promo

Hi folks! Our metasearch engine for Egyptian hieroglyphs is online. Before we explain what you can do with it, first a little promotional text ChatGPT wrote for us:

> Looking for a way to search for Egyptian hieroglyphs across multiple projects? Look no further than our website! Our unique metasearch engine allows you to search not only our own data, but also other projects like PNM, TLA, and Wikisource. No other search engine offers this level of comprehensive coverage for Egyptian hieroglyphs. And with some of these projects lacking their own search capabilities, our website is truly the only way to access all the information you need. Don't waste any more time sifting through incomplete search results - visit our website today and start exploring the world of Egyptian hieroglyphs like never before!

O.k. ;-) We would have written something like: "Annoyed that you have to search everything multiple times when searching in JSesh? Annoyed that you can't search for hieroglyphs in the new TLA? Then we have the solution! Our metasearch engine searches six Egyptological projects simultaneously for hieroglyphic writings."

![Search for hieroglyphs](/img/blog/search_for_hieroglyphs.jpg "MdC to Unicode converter")

## Real content

We've created two dedicated pages: <https://oraec.github.io/corpus/search/search_hieroglyphic_word_forms.html> and <https://oraec.github.io/corpus/search/search_hieroglyphs.html>. Why? Well, there are, after all, different targets in the search. Suppose a search is "𓄤𓆑" While one person wants only spellings of nfr, the other is also happy about the results like 𓃹𓈖𓈖𓄤𓆑𓂋𓅆 or 𓋴𓄤𓆑𓂋𓅱. So one searches for the spelling of a word form, while the other searches for the string, with any number of signs before or after it. That is why we implemented two searches: one for the word forms and the other for the hieroglyphic strings, in short: for the hieroglyphs. The second search returns more results than the first one. Understandable, isn't it?

The search for word forms imposes the following condition on the data: the word boundaries must be encoded. The data must not consist of a mere string of hieroglyphs. Not all data meet this condition. That means: some data are evaluated only in the search for hieroglyphs and not in the search for word forms.

## Projects

Our metasearch engine evaluates six Egyptological projects. We said a little about the selection criteria last time. Here are the individual projects.

### JSesh

[Serge Rosmorduc](https://github.com/rosmord) has published the texts of his program [JSesh](https://jsesh.qenherkhopeshef.org/) encoded in MdC in a [separate repository](https://github.com/rosmord/MDC-texts). We converted the freely licensed texts [last year](https://github.com/oraec/formerly-mdc-now_unicode/tree/main/jsesh). There is no delimitation of the word forms. Therefore, the data is only available for the second search. Compared to a normal search with ´´CTRL + F´´, our search has the advantage that the same characters are stored with the same code. It is always a bit annoying when you want to search for characters in JSesh. You have to search twice, once for m and once for G17. In our search one query is enough, more about that below.

### ORAEC

As the name says, [ORAEC](https://oraec.github.io/corpus) has a 'richly annotated corpus'. Some of the texts are annotated with hieroglyphs. Here the hieroglyphs are assigned to the individual word forms. We don't need to tell much more about ORAEC in this blog, do we?

### PNM

[PNM (Persons and Names of the Middle Kingdom)](https://pnm.uni-mainz.de/info) is a great project on onomastics and prosopography of the Middle Kingdom. It is interesting for our search engine that the project gives the respective writings for the different names.

### Ramsès

[Ramsès](http://ramses.ulg.ac.be/) is a digital corpus of Late Egyptian texts. The individual word forms are lemmatized and also encoded with hieroglyphs.

### TLA

The [TLA](https://thesaurus-linguae-aegyptiae.de/) is the most comprehensive digital corpus of Egyptian. This blog has already dealt extensively with the TLA. Some of the texts are annotated with hieroglyphs. Again, the hieroglyphs are associated with the word forms.

### Wikisource

The smallest corpus is that of [Wikisource](https://wikisource.org/wiki/Main_Page/Ancient_Egyptian). Word form boundaries are not available here.

This results in the following overview:

| Project | Search for word forms | Search for hieroglyphs |
| ------- | --------------------- |:----------------------:|
| JSesh   |           no          |          yes           |
| ORAEC   |           yes         |          yes           |
| PNM     |           yes         |          yes           |
| Ramsès  |           yes         |          yes           |
| TLA     |           yes         |          yes           |
| Wikisource|           no          |          yes           |

## Search

The search itself is kept quite simple. There is one input slot. You can enter MdC as well as Unicode. No matter if it says 'm', 'G17' or '𓅓', it will always search for '𓅓'. The input can contain more than one hieroglyph, e.g. 'k-Z4' or '𓈀𓏤'. As soon as you enter something, the search results are displayed. (O.k., sometimes you have to wait a bit at TLA because the searched file is so big). [AJAX](https://en.wikipedia.org/w/index.php?title=Ajax_(programming)&oldid=1152769494), we thank you!

The search results themselves are links to the respective project. At JSesh and at Wikisource the name of the text is the search result. The link leads to the text in our repo, so the user gets a readable Unicode view. At ORAEC, the word forms that match the search are displayed. The link leads to the summary page where all the occurrences for that writing are listed. For PNM and TLA, the results are counted through. There it says 'result #1', 'result #2', etc. As stated in the last blog, the hieroglyphic annotation in Ramsès is unfortunately not available in machine-readable form. Therefore there is only one link to the project. The link is only generated by a search for MdC. 

As said last time, the page really doesn't look pretty. But it works! We hope that it will be useful for you, dear readers!
