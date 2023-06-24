# ChatGPT and Egyptology - an experience report

Everyone is talking about ChatGPT. We don't need to explain what ChatGPT is, do we? ChatGPT is an AI with which you can have a conversation. The level of answers ChatGPT gives is so high that it is suspected of disrupting the writing professions. ChatGPT uses [LLM](https://en.wikipedia.org/w/index.php?title=Large_language_model&oldid=1161655735) to analyze huge amounts of existing data. ChatGPT processes what it is fed. Based on ChatGPT, many independent products have been developed in recent months. For example, [ChatPDF](https://www.chatpdf.com/) is useful: You upload a PDF and the AI can answer questions about the PDF and summarize the PDF. So you use the technology behind ChatGPT, but you use your own data for the evaluation.

Here we can take a bow to Egyptology. ChatGPT can't handle hieroglyphs (at least not today). What if you feed the technology with Egyptology data, just like you feed ChatPDF with any PDF? There are some tutorials on the web for this, e.g. <https://medium.com/@sohaibshaheen/train-chatgpt-with-custom-data-and-create-your-own-chat-bot-using-macos-fb78c2f9646d> But here you have to act on your own with a programming language, and the chat runs locally. That's why new services that promise a web-based solution are so attractive: You upload your data, the technology analyzes it, and you get a chatbot that responds based on your own data. Cool, right? One prominent service is [Chatbase](https://www.chatbase.co/). We report on our experience here in this blog.

Why did we choose Chatbase? Well, we were able to register with this service. It didn't work with [Chatfast](https://www.chatfast.io/). With [Fini](https://www.usefini.com/), you only get on the waiting list. And (the most important thing!) with Chatbase you can use the service for free. Many of the others require a paid subscription. The free offer at Chatbase differs from the paid ones in that it is more limited. The database of a free service at Chatbase can contain a maximum of 400k characters. In addition, only 30 (!) requests per month are possible with this chatbot. As you can see, this is a bit limited. But for a first try it should be enough!

After registering, you start feeding Chatbase with your data. You can upload files or select websites. We chose the second option. Our plan was to take all the data from <https://oraec.github.io/corpus>. In our [last blog](https://oraec.github.io/2023/06/22/oraec-search.html) we introduced our new search features. Will an AI be able to answer such questions? Will an AI be able to find all texts from Abydos? Back to setting up the chatbot! So we specified our website. Chatbase offers intelligent crawling: Chatbase does not only take the given URL, but searches all pages starting with the given URL, i.e. the pages related to the texts like <https://oraec.github.io/corpus/oraec1.html>, the digital editions like <https://oraec.github.io/corpus/oraec1_text.html>, the statistics pages like <https://oraec.github.io/corpus/oraec1_statistics.html>, and finally all overview pages. However, ORAEC is too big for Chatbase. The crawling stopped and did not cover all subpages! But also the crawled rest could not be integrated into the free chatbot, because the free chatbot can only contain up to 400k characters as a database. So we chose another strategy: we made a selection by taking the first 82 texts. We considered only the page with metadata and the page with statistics per text. These 164 web pages contain almost 400k characters in total, so the chatbot could be trained with this data.

![Chatbase: Data Sources; Crawl Websites](/img/blog/chatbase_add_website.jpg "Chatbase: Data Sources; Crawl Websites")

Now we wanted to test how well the chatbot works. The database consists of the texts oraec1, oraec2, oraec3 ... to oraec82. According to the review page <https://oraec.github.io/corpus/54VED6E3TBESLGFQGGQVXZ6GLM.html>, three of the first 82 texts date from the time of Merneptah: <https://oraec.github.io/corpus/oraec48.html>, <https://oraec.github.io/corpus/oraec63.html>, and <https://oraec.github.io/corpus/oraec73.html>. Can the chatbot find them? We give our test history here, with our questions in blockquotes and the answers in blocks of code:

> Could you tell me the texts which have the date "Merenptah"?

```
Certainly! There are two texts that have the date "Merenptah":

1. Ramses II - Merenptah: This text is referenced in KRI II, 2-101; KRITA II, 2-14; KRITANC II, 3-54; Birch, S./Hawkins, E. Select Papyri in the Hieratic Character from the Collections of the British Museum, Part I, Fasc. 1: Sallier Papyri; Budge, E.A.W., Facsimiles of Egyptian Hieratic Papyri in the British Museum, 2nd series; Kuentz, C., La Bataille de Qadech (MIFAO 55); Hassan, S., Le Poème dit de Pentaour et le rapport officiel sur la bataille de Qadesh; Möller, G., Hieratische Paläographie II; Davies, Egyptian Historical Inscriptions of the Nineteenth Dynasty (Documenta Mundi Aegyptiaca 2); and Gardiner, A.

2. Merenptah - Siptah u. Tausret: This text is referenced in Select Papyri in the Hieratic Character from the Collections of the British Museum, Vol. III; H. Brunner, Die Lehre des Cheti, Sohnes des Duauf, ÄgFo 13; W. Helck, Die Lehre des $Dwꜣ-Ḫtjj$, Kleine Ägyptische Texte; S. Jäger, Altägyptische Berufstypologien, LingAeg Studia monographica 4; and Redford, Egypt, Canaan and Israel in Ancient Times.

Is there anything else you would like to know?
```

That didn't work before. The chatbot returns only two texts and only bibliographic references. Let's take a closer look: The first hit is oraec48. The bibliographic references are incomplete: Entries are missing, and the existing entries omit the place of publication, year, and page number. The second hit is oraec73. Again, the bibliographic information is incomplete. There is even one entry here that is not present in oraec73, namely Redford, Egypt, Canaan, and Israel in Ancient Times. How did the chatbot come up with that? Very strange!

> Could you tell me the textnames and the ID (the string beginning with oraec and then following a number) of these texts with the date "Merenptah"?

```
Hmm, I am not sure.
```

Here we made the classic mistake of not asking in a structured enough way.

> Which texts have the date "Merenptah"? Please give in your answer following information: #1 the textname #2 the URL of the source

```
I apologize for any confusion, but as an AI language model, I don't have direct access to specific URLs or sources. However, based on the information provided, I can tell you that there are two texts mentioned with the date "Merenptah":

1. Ramses II - Merenptah: The source references for this text include KRI II, 2-101; KRITA II, 2-14; KRITANC II, 3-54; Birch, S./Hawkins, E. Select Papyri in the Hieratic Character from the Collections of the British Museum, Part I, Fasc. 1: Sallier Papyri; Budge, E.A.W., Facsimiles of Egyptian Hieratic Papyri in the British Museum, 2nd series; Kuentz, C., La Bataille de Qadech (MIFAO 55); Hassan, S., Le Poème dit de Pentaour et le rapport officiel sur la bataille de Qadesh; Möller, G., Hieratische Paläographie II; Davies, Egyptian Historical Inscriptions of the Nineteenth Dynasty (Documenta Mundi Aegyptiaca 2); and Gardiner, A.

2. Merenptah - Siptah u. Tausret: The source references for this text include Select Papyri in the Hieratic Character from the Collections of the British Museum, Vol. III; H. Brunner, Die Lehre des Cheti, Sohnes des Duauf, ÄgFo 13; W. Helck, Die Lehre des $Dwꜣ-Ḫtjj$, Kleine Ägyptische Texte; S. Jäger, Altägyptische Berufstypologien, LingAeg Studia monographica 4; and Redford, Egypt, Canaan and Israel in Ancient Times.

If you have access to the mentioned sources, you may be able to find more specific information about the text names and corresponding URLs.
```

Exciting, right? The chatbot returns the same answer as the first time, so again only two hits instead of three. It seems that the training does not store the original URL of the data, so the chatbot is overwhelmed by the question about the URL of the data. The fact that the AI does not output the text name is very surprising, because it is explicitly in the HTML files. So the next try:

> You mentioned the source references, but there is more metadata. Could you please tell me the entire metadata of the texts with the date "Merenptah"?

```
Certainly! I apologize for the oversight. Here are the complete metadata details for the texts with the date "Merenptah":

1. Ramses II - Merenptah:
   - Textname: Not specified in the given information.
   - Source: KRI II, 2-101; KRITA II, 2-14; KRITANC II, 3-54; Birch, S./Hawkins, E. Select Papyri in the Hieratic Character from the Collections of the British Museum, Part I, Fasc. 1: Sallier Papyri; Budge, E.A.W., Facsimiles of Egyptian Hieratic Papyri in the British Museum, 2nd series; Kuentz, C., La Bataille de Qadech (MIFAO 55); Hassan, S., Le Poème dit de Pentaour et le rapport officiel sur la bataille de Qadesh; Möller, G., Hieratische Paläographie II; Davies, Egyptian Historical Inscriptions of the Nineteenth Dynasty (Documenta Mundi Aegyptiaca 2); and Gardiner, A.

2. Merenptah - Siptah u. Tausret:
   - Textname: Not specified in the given information.
   - Source: Select Papyri in the Hieratic Character from the Collections of the British Museum, Vol. III; H. Brunner, Die Lehre des Cheti, Sohnes des Duauf, ÄgFo 13; W. Helck, Die Lehre des $Dwꜣ-Ḫtjj$, Kleine Ägyptische Texte; S. Jäger, Altägyptische Berufstypologien, LingAeg Studia monographica 4; and Redford, Egypt, Canaan and Israel in Ancient Times.

Please note that the specific text names and additional metadata details may be available within the mentioned sources.
```

Wow, that was nothing again. Interestingly, the internal view where we did the chat lists the three texts oraec48, oraec63, and oraec73, which are the hits. Unfortunately, we did not take a screenshot of them.

The conclusion of this experiment is that the chat is unusable because it does not find all the hits and cannot specify the desired metadata. Shockingly, the chatbot invents an additional bibliographic specification. In this respect, our chatbot is completely worthless (at the moment, at this stage of training).

If you like, you can give the bot a try. Have a look at <https://oraec.github.io/corpus/search/>. But keep in mind that the chatbot can only handle 30 requests per month. So set your alarm at the beginning of the month ;-)
