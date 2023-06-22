# ORAEC Search

We had created a [roadmap](https://oraec.github.io/2023/05/05/roadmap-and-preliminary-work-for-a-hieroglyphic-metasearch-engine.html). Do you remember? We want to enable search in ORAEC. But our goal is not a perfect search interface. We want to give you the tools to build your own search interface - according to your individual needs. Such a toolbox is now ready; we present it to you now. To give you a better understanding of the toolbox, we have published individual searches ([here](https://oraec.github.io/corpus/search/oraec_metadata_search.html), [here](https://oraec.github.io/corpus/search/oraec_parameter_search.html), and [here](https://oraec.github.io/corpus/search/oraec_combined_search.html)) as a kind of proof of concept.

But first, some general remarks: What does it actually mean to search a corpus? What does it mean in concrete terms? In general: You have a question about a corpus. The search should produce a hit list of elements from the corpus that can answer the question. The questions can be very different: simple, like a search for all texts on ostraca, or complex, like a search for all texts from the Old Kingdom in which the infinitive of a verb is written with an ending. They can differ in their [granularity](https://en.wikipedia.org/w/index.php?title=Granularity&oldid=1151382901). One can search specifically for texts from the reign of a particular pharaoh, or one can search more broadly for texts from a dynasty or era. This is one of the difficulties in designing search interfaces. One tries to answer as many questions as possible. In addition, the search should be user-friendly.

A high standard, isn't it? So how do you proceed strategically? A powerful tool for a search is an own [query language](https://en.wikipedia.org/w/index.php?title=Query_language&oldid=1161279846). You probably know the [Coptic Scriptorium](https://copticscriptorium.org/). The connected tool [ANNIS](https://annis.copticscriptorium.org/annis/scriptorium) uses such a query language. It can be used to answer practically any question. But for a user, who searches there only occasionally something, is not comfortable at all. Such a language has to be learned separately. You cannot start intuitively. As powerful as a query language is: it is unfortunately also very daunting. We could build a query language for ORAEC. But this should not be the first and not the only approach, because casual users cannot handle it. The other extreme is the simple search slot we all know from Google. That's what we're all used to. That's ideal for a lot of data that can be structured very differently. Then it's best to do a full-text search and use a simple search slot. If the data can be structured differently, you don't know what to expect. If you want to search for "KMT", you may want to search for the word for Egypt, or you may want to search for the journal. A full-text search with a simple search slot can be completely agnostic and simply return all hits. ORAEC, on the other hand, has structured data. Egyptian words are marked as words, bibliographic data are marked as bibliographic data. This structuring is a great advantage to exploit. A full text search for "Seth" would possibly also find the Egyptologist "Sethe". If one specifies in which area one wants to search "Seth", one minimizes the false positives. In this respect we do not want to offer a simple search slot, but several search slots, each responsible for one area. For another advantage see below!

O.k., so multiple search slots for multiple areas. What do we mean by areas now? These are the respective properties, e.g. date or find spot. We have to distinguish between two types of properties: There are properties that apply to an entire text, i.e. the find spot or the object type. There are also properties that apply only to a specific word, i.e. to a specific token. A token can be a sḏm.n=f. This does not mean, however, that the entire text consists only of sḏm.n=f. These different types also entail different types of hit lists. If you search for a certain property of a token, e.g. all sḏm.n=f, then you want to get these tokens as result and not the text. What is the benefit if you know that in [oraec1](https://oraec.github.io/corpus/oraec1.html) a sḏm.n=f is used? You want to know the exact location of the sḏm.n=f! It is different with the properties that apply to the entire text. Here you want to get as hits all texts which have a certain property. O.k., so again: once there are properties of a text. If you search for them, you should also get texts as hits. Besides there are the properties of the single tokens. If you search for them, you should get these tokens and not the whole text. We concluded that we need two different searches, one for the metadata, where you get texts as hits, and one for the parameters, where you get tokens as hits. The search for metadata includes the fields that apply to the entire text. The search for parameters contains the fields which concern single tokens. So, to take an example from above, a search for all texts on ostraca is a search for the metadata. A search for nouns in plural and status constructus is a search for parameters. Above we had also given the following example: a search for all texts from the Old Kingdom in which the infinitive of a verb is written with an ending. Here we have properties concerning the whole text as well as properties concerning single tokens. In addition, we have created a third search that combines the search for metadata and the search for tokens. And since we only want to provide a proof of concept, we only included three search slots in one search. If you want other search slots or more, look below for the technical details!

With these three searches using multiple search slots, we can perform both simple and complex searches. However, we only map the Boolean AND, i.e., the hit list only consists of hits that match all the properties we are looking for. A Boolean OR or a Boolean NOT does not work with our simple search slots. More specifically, it does not work with our proof of concept. Of course, you can modify the script accordingly. See below for possibilities.

Where to search now? We have created separate files for the different properties, which are located in the subfolder "search" of branch "gh-pages" of the repo corpus, cf. <https://github.com/oraec/corpus/tree/gh-pages/search>. The name of the file tells you what type of property it is. The properties that affect the whole text start with "metadata_search_". These are [metadata_search_author.json](https://github.com/oraec/corpus/blob/gh-pages/search/metadata_search_author.json), [metadata_search_date.json](https://github.com/oraec/corpus/blob/gh-pages/search/metadata_search_date.json), [metadata_search_location.json](https://github.com/oraec/corpus/blob/gh-pages/search/metadata_search_location.json), [metadata_search_objecttype.json](https://github.com/oraec/corpus/blob/gh-pages/search/metadata_search_objecttype.json) and [metadata_search_origplace.json](https://github.com/oraec/corpus/blob/gh-pages/search/metadata_search_origplace.json). The properties that only affect individual tokens start with "some_parameter_": [some_parameter_genus](https://github.com/oraec/corpus/blob/gh-pages/search/some_parameter_genus.json), [some_parameter_hiero](https://github.com/oraec/corpus/blob/gh-pages/search/some_parameter_hiero.json), [some_parameter_inflection](https://github.com/oraec/corpus/blob/gh-pages/search/some_parameter_inflection.json), [some_parameter_lemma_form](https://github.com/oraec/corpus/blob/gh-pages/search/some_parameter_lemma_form.json), [some_parameter_lemmaID](https://github.com/oraec/corpus/blob/gh-pages/search/some_parameter_lemmaID.json), [some_parameter_numerus](https://github.com/oraec/corpus/blob/gh-pages/search/some_parameter_numerus.json), [some_parameter_pos](https://github.com/oraec/corpus/blob/gh-pages/search/some_parameter_pos.json), [some_parameter_status](https://github.com/oraec/corpus/blob/gh-pages/search/some_parameter_status.json), [some_parameter_verbalClass](https://github.com/oraec/corpus/blob/gh-pages/search/some_parameter_verbalClass.json) and [some_parameter_voice](https://github.com/oraec/corpus/blob/gh-pages/search/some_parameter_voice.json). These files are extracted from the source data located in <https://github.com/oraec/corpus_raw_data>. We did not extract every property. The properties "pronoun" or "morphology" are missing. If you need them, you can easily get them from the source data. The files themselves are quite simple. They are a simple dictionary. The keys are the values that a particular property can take. So there is "participle" as a possible inflection. So "participle" is a key in some_parameter_inflection.json. The values are then the elements that have the property of the key. The key "participle" has as value all tokens marked as participle. The advantage of these prepared files is that you can quickly find exactly what you are looking for.

The next point of general preliminary remarks is granularity. The texts in ORAEC are either very finely dated in the reign of a pharaoh, or somewhat more roughly dated in a particular dynasty, or very roughly dated in a particular era. If we are looking for Old Kingdom texts, we should also find the texts that have the very fine dating "Khufu". This means that we need to modify the metadata_search_date.json file. Texts with the dating "Khufu" must be additionally listed with the keys for the 4th Dynasty and for the Old Kingdom. With this enrichment we can guarantee that the texts with a fine-grained dating will be found even when searching for an epoch. We have done a similar enrichment for provenance. Finally, our controlled vocabulary is based on <https://github.com/simondschweitzer/aed-tei/blob/master/files/thesaurus.xml>, the thesaurus of the AED. The thesaurus sorts its entries hierarchically. The find spot entries depend on a total of 13 root nodes: "Niltal südlich des 3. Katarats bis zum 4. Katarakt", "(unbestimmt)", "Nildelta", "Niltal südlich des 1. Katarakts bis zum 2. Katarakt", "Wüste östlich des Niltals und Küste des Roten Meeres (Staatsgebiet Ägypten und Sudan)", "Niltal südlich von Assiut bis zum 1. Katarakt", "Niltal von Kairo bis Assiut", "Niltal südlich des 2. Katarakts bis zum 3. Katarakt", "Wüste westlich des Niltals (Staatsgebiet Ägypten und Sudan)", "Niltal südlich des 4. Katarakts bis Chartum", "Nordafrika", "Vorderasien und Europa" and "(unbekannt)". We have now enriched the values of these root nodes with all subordinate entries. So a search for "Nile Delta" will also find the entries that represent a specific location of the delta.

Great! So we have three search pages with different search slots. The big problem with search slots is that you never know what the entries are supposed to look like. Is it "Saqqara" or "Sakkara"? Is it "Fayyum" or "Fajjum" or something else? To solve this problem, there is [autocomplete](https://en.wikipedia.org/w/index.php?title=Autocomplete&oldid=1159407117). When you start to fill in a field, you get suggestions of what you can type. For example, if you type "Sa" in the find spot field, you will be offered "Saqqara". You can click on this value to avoid typos. An ingenious feature that we love! The suggestion list itself is sorted alphabetically, but the dates are sorted chronologically.

O.k., before we get too technical, let's summarize the most important thing: we now have three [search pages for ORAEC](https://oraec.github.io/corpus/search/). On the [first page](https://oraec.github.io/corpus/search/oraec_metadata_search.html) you can search for text in the fields objecttype, date and findspot. On the [second page](https://oraec.github.io/corpus/search/oraec_parameter_search.html) we can search for single words, namely for the word, for the inflection and for the verbal class. The [third search](https://oraec.github.io/corpus/search/oraec_combined_search.html) combines these two. For those who want to customize these searches, stay tuned and read the rest of the technical stuff. For everyone else, thank you for stopping by. We hope you enjoy our search pages!

How does our search work? It's a simple HTML page with Javascript handling JSON data. That's about it. Let's take a look at the metadata search first: <https://github.com/oraec/corpus/blob/gh-pages/search/oraec_metadata_search.html>. The body is just:

```
<body>
<h1>ORAEC metadata search</h1>
<input type="text" id="input1" placeholder="Enter an objecttype">
<input type="text" id="input2" placeholder="Enter a date">
<input type="text" id="input3" placeholder="Enter a findspot">
<button id="submit">Search!</button>
<p class="source">ORAEC's proof of concept of a metadata search</p>
<h2>Results</h2>
<div id="results"></div>
<p class="author">Data Authors: Burkhard Backes, Susanne Beck, Marc Brose, Adelheid Burkhardt, Roberto A. Díaz Hernández, Peter Dils, Roland Enmarch, Frank Feder, Heinz Felber, Silke Grallert, Stefan Grunert, Ingelore Hafemann, Anne Herzberg, John M. Iskander, Ines Köhler, Renata Landgrafova, Verena Lepper, Lutz Popko, Alexander Schütze, Stephan Seidlmayer, Gunnar Sperveslage, Susanne Töpfer, Doris Topmann, Altägyptisches Wörterbuch<br />Source: <a href="https://oraec.github.io/corpus/">ORAEC</a> (cc-by-sa-4.0)<br />Created by ORAEC</p>
</body>
```

We have defined three input fields that can be addressed with their respective IDs. After clicking the button the search is started, which is defined here in `script`. The code is included in the HTML page. We only use the [jQuery](https://jquery.com/) library for the autocomplete function. Let's see what happens when the button is clicked:

```
$(document).ready(function() {
$("#submit").click(function() {
var input1 = $("#input1").val();
var input2 = $("#input2").val();
var input3 = $("#input3").val();

$.when(
$.getJSON("metadata_search_objecttype.json"),
$.getJSON("metadata_search_date.json"),
$.getJSON("metadata_search_origplace.json")
).done(function(data1, data2, data3) {
var result = [];

let tempResult1 = [];
let tempResult2 = [];
let tempResult3 = [];
let boole1 = true;
let boole2 = true;
let boole3 = true;
```

The values entered in the fields are saved as input1, input2 and input3. Then the JSON files to be searched are loaded and temporary variables are defined.

Now the input is matched with the data from the JSON files:

```
if (input1.length > 0) {
if (data1[0][input1]) {
tempResult1 = data1[0][input1];
}
} else {
boole1 = false;
}
```

First it is checked if the field is filled in at all. If not, this case is not to be considered. Then the temporary variable gets the Boolean value `false`. If there is now an input in the field, it is checked if this value exists in the JSON file. If so, the value from the JSON is stored as a temporary result. If not, nothing happens. This process is applied to the three fields. So there are up to three temporary results and up to three Boolean variables. After all, we are looking for the texts that match all the conditions. I.e. we have a Boolean AND and we search the intersection of the temporary results. The Boolean variable indicates whether a field must be included in the intersection. The final intersection set is stored as `result`.

```
if (result.length > 0) {
var oraeclink = "<a href=\"https://oraec.github.io/corpus/";
sequence = [];
for (i in result) {
check = oraeclink.concat(result[i], ".html\">", result[i], "</a>")
sequence.push(check)
}
document.getElementById("results").innerHTML = sequence.join(", ");
} else {
document.getElementById("results").innerHTML = "Sorry! No results!";
}
```

If `result` is not empty, the results are generated as links. Otherwise, the output is "Sorry! No results!"

Finally, the autocomplete:

```
$("#input1").autocomplete({
source: function(request, response) {
$.getJSON("metadata_search_objecttype.json", function(data) {
var filteredData = $.grep(Object.keys(data), function(element) {
return element.indexOf(request.term) !== -1;
});

response(filteredData);
});
},
minLength: 1
});
```

Important here is the definition of which field it is: `$("#input1")`, and the specification of the underlying file `$.getJSON("metadata_search_objecttype.json", function(data) {`. Autocomplete must be defined for each field separately.

The search for parameters is built exactly the same way. The only difference is the creation of the links for the results. The tokens are displayed, but the link goes to the sentence containing the token. The single result here is `check = oraeclink.concat(result[i].split("-")[0], "-", result[i].split("-")[1], ".html\">", result[i], "</a>")`. That generates - for example - a `<a href="https://oraec.github.io/corpus/oraec1449-2.html">oraec1449-2-3</a>`.

The combined search first performs a search for the metadata and a search for the parameters separately. It then returns those tokens from the parameter search that occur in texts from the metadata search result set.

As you can see, this is all very simple. As I said, this is just a proof of concept. It doesn't look pretty, does it? But we think it works. We hope you can do something with it and that you find many texts with these searches!

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a></p>
