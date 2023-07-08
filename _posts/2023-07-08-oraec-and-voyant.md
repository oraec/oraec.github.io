# ORAEC and Voyant

So, folks, let's make good on our next promise! We quote from our [roadmap](https://oraec.github.io/2023/05/05/roadmap-and-preliminary-work-for-a-hieroglyphic-metasearch-engine.html):

> We want to provide a text analysis tool for the ORAEC data.

## Text analysis tool

What is a text analysis tool? Well, a text analysis tool provides information like we offer on [our statistics pages](https://oraec.github.io/2023/02/02/text-statistics.html), such as the most frequent words. It also does [text mining](https://en.wikipedia.org/w/index.php?title=Text_mining&oldid=1153309534). Such text analysis tools are a dime a dozen. Which one should we use for ORAEC? We considered the following selection criteria:

* The tool should be language independent; it should be able to handle Egyptian language data. (You wouldn't believe how many tools specialize only in English).
* It should be able to handle hieroglyphs in Unicode.
* It should be easy to use.
* It should have a web interface. If possible, there should also be a version that can be run locally.
* It should have good display options, like [KWIC](https://en.wikipedia.org/w/index.php?title=Key_Word_in_Context&oldid=1153811801).
* It should have search capabilities.
* It should allow evaluations, such as [topic modeling](https://journalofdigitalhumanities.org/2-1/topic-modeling-a-basic-introduction-by-megan-r-brett/).

## Voyant

It was based on these criteria that we ended up with [Voyant](https://voyant-tools.org/). According to <https://doi.org/10.1093%2Fllc%2Ffqv052>, Voyant Tools 

> was conceived to enhance reading through lightweight text analytics such as word frequency lists, frequency distribution plots, and KWIC displays.

This isn't the place to give a general introduction to Voyant. Have a look here <https://lib.murraystate.edu/ld.php?content_id=61330394> or go directly to the detailed help pages <https://voyant-tools.org/docs/#!/guide/tools> or <https://voyant-tools.org/docs/>. This blog will show you what you can do with ORAEC data in Voyant.

Dear readers, if you follow our project history, you know that we started with representing hieroglyphs in Unicode and that this has always been our focus. In this context, we decided to feed Voyant not with Egyptological transcriptions, but with Egyptian hieroglyphs. So we generated txt files from our raw data, consisting entirely of hieroglyphic text. Unlike our repository <https://github.com/oraec/formerly-mdc-now_unicode>, which contains Egyptian text in hieroglyphs, the texts are tokenized; that is, the word forms are separated by spaces. Also, one line represents one sentence. Finally, there is information about the source, authorship, and license. Here is an example:

```
𓌢𓈖𓌢𓈖 𓁹 𓂋 𓄣 𓅮 𓌸𓇋𓇋
𓊃 𓇋𓅓𓂜 𓎡 𓇋𓅓𓐛 𓁹 𓂋 𓇑𓇑
Source: https://github.com/oraec/corpus_raw_data/blob/main/oraec2892.json
Credits: {"license"=>"cc-by-sa-4.0", "author"=>"Stefan Grunert", "source"=>["https://github.com/simondschweitzer/aes", "https://github.com/simondschweitzer/aed-tei/blob/master/files/WCJ3EC3YJJD27DDAGSESNQHVYY.xml"]}
```

These txt files should be the basis for use in the text analysis tool Voyant. They are in a separate repository: <https://github.com/oraec/text-analysis-data>. We have uploaded this corpus to the text analysis tool mentioned above. Thus, Voyant now has an instance of Egyptian texts that is freely accessible to anyone: <https://voyant-tools.org/?corpus=1d596abab535000991688f8d672fcee2&lang=en>. Bookmark it!

## ORAEC Data in Voyant

### Overview

When you click on the link, you will see a web page with five sections:

![Voyant: Start](/img/blog/voyant_corpus_overview.jpg "Voyant: Start")

In the upper left corner is a word cloud created from all word forms of all texts. The larger the word, the more often it is used.

In the middle, you can read through all the texts in the corpus. Voyant displays them as continuous text.

The upper right corner shows the trends. Four selected words are represented by four colored dots. The position in the coordinate system is determined by the relative frequency of the words in the individual texts. You can also display the distribution of the relative frequency of a self-selected word.

![Voyant: Trends](/img/blog/voyant_corpus_trends.jpg "Voyant: Trends")

On the bottom left there is a summary of the corpus: number of texts, number of tokens, number of types, length of texts, vocabulary density, etc. There is also an overview of the keywords of a text:

![Voyant: Distinctive Words](/img/blog/voyant_corpus_summary_distinctive_words.jpg "Voyant: Distinctive Words")

On the bottom right is the [KWIC](https://en.wikipedia.org/w/index.php?title=Key_Word_in_Context&oldid=1153811801) view, something we wanted in our selection criteria. KWIC means "key word in context" and is a listing of all evidence for a word in its context. The word is displayed in the middle. To the left are the words that immediately precede it in a document, and to the right are the words that follow it. At the bottom left, you can change the view by typing a word.

![Voyant: KWIC](/img/blog/voyant_corpus_kwic.jpg "Voyant: KWIC")

As you can see in the figure, you don't have to type a complete word form. Even a 𓊹* is provided. Here * is a wildcard. So 𓊹* will select all word forms that start with 𓊹:

![Voyant: Context](/img/blog/voyant_corpus_context.jpg "Voyant: Context")

But this is only the start page. We cannot present everything, but limit ourselves to what is most fruitful from an Egyptological point of view.

### Cluster analysis

The ScatterPlot creates a representation of texts and words in a coordinate system that is intended to visualize the relationships between the texts themselves, but also between the texts and the words. You can perform a [correspondence analysis](https://en.wikipedia.org/w/index.php?title=Correspondence_analysis&oldid=1155294612)

![Voyant: CA](/img/blog/voyant_corpus_scatterplot.jpg "Voyant: CA")

or a [principal component analysis](https://en.wikipedia.org/w/index.php?title=Principal_component_analysis&oldid=1160912942)

![Voyant: PCA](/img/blog/voyant_corpus_scatterplot_pca.jpg "Voyant: PCA")

or an analysis of the similarity of the different texts

![Voyant: Document Similarity](/img/blog/voyant_corpus_scatterplot_document_similarity.jpg "Voyant: Document Similarity")

### Collocates

Collocates lists the collocations in the corpus: Which two word forms occur together in a sentence?

![Voyant: Collocates](/img/blog/voyant_corpus_collocates.jpg "Voyant: Collocates")

### Documents

This is an overview of the texts in the corpus: Number of tokens of a text, number of types of a text, the TTR (see [our blog](https://oraec.github.io/2023/02/09/type-token-ratio.html) for more information). With Modify you can remove texts from the corpus and also add other texts. See below for uploading!

![Voyant: Documents](/img/blog/voyant_corpus_documents.jpg "Voyant: Documents")

### Phrases

"Phrases" lists the combinations of word forms that occur more than once in the corpus. You can sort by phrase length or by the number of words involved.

![Voyant: Phrases](/img/blog/voyant_corpus_phrases.jpg "Voyant: Phrases")

### Terms

This table lists the words of the corpus sorted by their frequency and shows their number. The column "Trends" visualizes in which texts the words appear frequently or rarely.

![Voyant: Terms](/img/blog/voyant_corpus_terms.jpg "Voyant: Terms")

For each word there is a detailed view with distribution, collocates, correlations, and phrases.

![Voyant: Terms Detail](/img/blog/voyant_corpus_terms_detail.jpg "Voyant: Terms Detail")

### Topic Modeling

Voyant can also do [topic modeling](https://en.wikipedia.org/w/index.php?title=Topic_model&oldid=1160027774). It creates different topics represented by the words. Next to them you can see the distribution of these topics within the texts.

![Voyant: Topic Modelling](/img/blog/voyant_corpus_topics.jpg "Voyant: Topic Modelling")

### Word Tree

This visualizes which words typically come before and after a particular word.

![Voyant: Word Tree](/img/blog/voyant_corpus_wordtree.jpg "Voyant: Word Tree")

You surely know this from the [Coptic Dictionary Online](https://coptic-dictionary.org/), don't you?

## Local Voyant Server

Voyant is really awesome, isn't it? There is a problem with the web service: the ORAEC data are too numerous to be processed completely. <https://voyant-tools.org/?corpus=1d596abab535000991688f8d672fcee2&lang=en> only provides the hieroglyphically annotated texts up to [oraec2991](https://oraec.github.io/corpus/oraec2991.html). But if you want to analyze all texts with Voyant, you have to install the [Voyant Server](https://github.com/voyanttools/VoyantServer). This is a small JAVA program that generates a view in your browser that is identical to the view from the web.

Then you have to go to the settings and make two changes: Under "Text" there is an item "omit from". Please enter `Source:` there. This is because the files contain the source information (which is not needed for text analysis) as well as the hieroglyphic text. Furthermore, there is the item "Processing". Please select the value `Whitespace Only` in the field "Tokenization". This will make the tokenization work best.

![Voyant: Options](/img/blog/voyant_corpus_options.jpg "Voyant: Options")

You can then use the Upload button to upload files from your local computer (for example, our downloadable ORAEC data). Once uploaded, all ORAEC texts are ready for analysis in Voyant. Have fun!

## Alternatives

In addition to Voyant, we also recommend [Lexos](http://lexos.wheatoncollege.edu/). We prefer Voyant for three reasons: First, Lexos has no simple URL to share the instance with the ORAEC data. Instead, you have to upload the data yourself. Second, there is no KWIC view. Third, you can run Lexos locally, just like Voyant, but installing a local Lexos is a bit complicated. However, Lexos offers one feature not found in Voyant. Lexos can dendrogram the coherence of the texts:

![Lexos: Dendrogram](/img/blog/lexos_dendrogram.jpg "Lexos: Dendrogram")

So if you like the visualizations of Lexos, the best thing to do is to use [this file](https://github.com/oraec/text-analysis-data/raw/main/lexos/oraec.lexos) in Lexos, which contains all the ORAEC data.

## Conclusion

With these text analysis tools, especially Voyant, you can create sophisticated analyses: Keywords, text associations, or even topic modeling, to name just a few. With the ORAEC data, Egyptian corpus data is available. Now it's your turn! Take advantage of the new possibilities and gain new insights from this material!

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a></p>
