# Roadmap and preliminary work for a hieroglyphic metasearch engine

Hi folks! We are back! It's been a very long time since we've been in touch. There have been some personnel changes as well. Thank you very much, dear people, for being involved in this project! A special thank you goes to Angela and Stevie! (You already know for what...).

When we got back together after Easter, we created a roadmap of what we want to do in the near future. This plan consists of three points: We want to create a metasearch engine that searches the hieroglyphic writing of various digital projects. We want to publish a construction kit for a search interface of our ORAEC data. We want to provide a text analysis tool for the ORAEC data.

First to the first point! We have some preliminary work on this as well, which is why we dare to publish this blog now. What do we mean by "metasearch engine"? We want to search simultaneously in several digital Egyptological projects! The idea is: you type in a hieroglyphic writing once, and the metasearch engine returns the results from the different projects in one place! Cool, isn't it?

As a starting point, we can take the data we converted last year: [Wikisource](https://oraec.github.io/2022/10/01/converting-manuel-de-codage-to-unicode.html), [JSesh](https://oraec.github.io/2022/10/10/missing-unicode-characters-and-further-mapping-problems.html), and of course [AES](https://oraec.github.io/2022/10/14/four-challenges-when-converting-aes.html), which is the foundation of our ORAEC data. For ORAEC, we already have an [overview page of all writings](https://oraec.github.io/corpus/all_writings.html) that we can reuse. What about other projects and their data?

The easiest and best way is for projects to publish their data. Then reuse is easy to arrange. This is the case in the fantastic project [Persons and Names of the Middle Kingdom](https://pnm.uni-mainz.de/info). The data is published on Zenodo under the cc-by license. We were able to very quickly extract the data, optimize it for search, and most importantly convert it to Unicode. Our JSON is structured as follows: a writing is the key, the associated values are the URLs where the writing is encountered in the PNM project.

If no raw data is published, one must hope that at least on the individual web pages of a project, the hieroglyphic writings are encoded not only as images, but also as data (MdC or Unicode). This is the case with the [new TLA](https://thesaurus-linguae-aegyptiae.de/). You can see the images on the surface, but the source code of a web page provides the associated MdC code. We have now scraped all the lemmatized sentences from the TLA. In the [last blog](https://oraec.github.io/2023/02/20/lifting-a-treasure-web-scraping-of-the-new-tla.html), we described the procedure for the demotic texts. We adapted that for the Egyptian sentences. From this we were able to create a large table of which writing occurs in which sentence. In [our review of the new TLA](https://oraec.github.io/2022/11/16/review-of-the-new-tla-part-three.html#hieroglyphic-writing) we complained that the hieroglyphic writings in the TLA are understood as facsimiles rather than as digital data. Therefore, we had to invest a lot of time for data cleaning. Finally, we were able to upload the [result](https://github.com/oraec/scraped_data/blob/main/new_tla/egyptian/hieroglyphic_writings_new_tla_in_unicode.json) to our repository of web scraping data. Each writing has the IDs of the sentences in which it occurs.

Then there are projects that publish the hieroglyphic writings as images but do not provide the code behind them, e.g. [Karnak](http://sith.huma-num.fr/karnak). This project publishes inscription located in the temple of Karnak. The website only provides png files for the hieroglyphic writings. We had briefly considered doing a bit of reverse engineering on this, i.e. running OCR over the images. But that would have been a separate project and would have taken a lot of time. So there are promising approaches for OCR with hieroglyphics, but nothing seems to be directly reusable to us. Or have we missed something? We know the approaches of [Mark-Jan Nederhof](
https://nbn-resolving.org/urn:nbn:de:bsz:15-qucosa-201704), [PySesh](https://github.com/D-K-E/PySesh), [Glyphnet](https://github.com/GAIA-IFAC-CNR/Glyphnet) and [Anton Alekseev](https://github.com/alexeyev/glyphnet-pytorch). In addition, there is a [thesis](https://doi.org/10.6082/uchicago.3695) on OCR for the hieratic that is worth reading. Back to the actual topic: Such projects, which only offer images, are currently out of the question for our metasearch engine.

Finally, there is [Ramsès](http://ramses.ulg.ac.be/), the digital corpus of Late Egyptian texts. As in the Karnak project, hieroglyphic writings are offered exclusively as images, e.g. <http://ramses.ulg.ac.be/spelling/img/47208>. But Ramsès (unlike Karnak or the new TLA) allows us to search for hieroglyphic writings: <http://ramses.ulg.ac.be/search/mdc?request=m-r>. The search query is thus mapped in the URL. This allows us to easily forward our searches to Ramsès.

We anticipate one of your questions here: What about [API](https://en.wikipedia.org/w/index.php?title=API&oldid=1153040652)? This is generally a good idea; because an API is made for a website to offer its data for targeted queries. Now comes the big but: the projects we want to query with our metasearch engine don't have APIs. In the Egyptological context, an API is not yet a given, but rather rare. [THOT](http://thot.philo.ulg.ac.be/index.html), for example, has such an access. But even if some projects had such an API, it would not be a big success for metasearch engine of hieroglyphic writings. A lot of data cleaning is necessary to search the data in a meaningful way. An API probably makes more sense in a standardized environment, such as with THOT's thesauri. The data collection of the hieroglyphic writings is unfortunately more than wild and has to be reworked a lot for a reuse. (We refrain from our favorite quote from Mark-Jan Nederhof).

Now we just need to create a search interface. We're not designers; it won't look very pretty, but hopefully the search will work. Stay tuned!

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a></p>
