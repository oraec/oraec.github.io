# Review of hieroglyphs.ai

Another review today! But don't worry, it won't be super long!

Recently there was a mail on the [EEF mailing list](https://www.egyptologyforum.org/EEFNEWS.html) introducing an app. It's called [Hieroglyphs AI Android app](https://play.google.com/store/apps/details?id=ai.hieroglyphs.hieroglyphs_ai) and promises to recognize hieroglyphs as characters from pictures. We didn't look at the app, but at the service, which is available at <https://hieroglyphs.ai>.

We cite the About page there:

> Hieroglyphs AI allows you to automatically identify the Gardiner codes of hieroglyphs contained in image files on your computer using a deep convolutional neural network.
> Click the screen, hold the left mouse button and move the mouse to draw a square enclosing the hieroglyph of interest. To be recognized, an Egyptian sign should be approximately in the middle of the selected area and should be represented in full (without cutoff).
> The neuronal net was trained on a dataset that contains 1000 images in each of the 366 classes of hieroglyphs.

That doesn't sound bad, does it? And we predict the result: it actually works quite well! But first, a general note. We want to distinguish between two areas of application: First, you have images of Egyptian objects with hieroglyphs, i.e. images of original artifacts. Second, there are hieroglyphs in books or articles. Nowadays, these hieroglyphs are created with a computer-generated font, sometimes even as Unicode. In the past, however, hieroglyphs were often handwritten, for example in the " Urkunden ". We call this kind of hieroglyph recognition retro-digitization, while we call the first case digitization. We expect the recognition in retro-digitization to be better than in digitization because it is already standardized. So, to test our hypothesis, we need an object that has both a photo and a computer-generated transcript, preferably freely available! Have a look here:

![Test text Wikisource](/img/blog/wikisource_senusret.jpg "Test text Wikisource")

We simply took the [first text from Wikisource](https://wikisource.org/w/index.php?title=Stelae_of_the_caretaker_Senusret&oldid=276103), a stele that is now in the Louvre. Here you can see the computer generated hieroglyphs that Wikisource uses. In addition, Wikisource provides a [photo of the original](https://commons.wikimedia.org/w/index.php?title=File:Egypte_louvre_272_stele.jpg&oldid=619070409). So we have a test possibility of the same text, once in the original and once with computer generated hieroglyphs.

However, the font used by Wikisource is not used in Egyptological publications. At least we are not aware of it. Maybe you know? It would be nice if this test text were also available with the more common computer generated hieroglyphs. In the past the hieroglyphs were set with the software Winglyph. See also the volumes of Jansen-Winkeln, Inschriften der Spätzeit. All this is done with Winglyph! Since some time there is a free version on the internet called Webglyph: <http://71.174.62.16/Demo/WebGlyph2> There we created the test text with the Winglpyh hieroglyphs. Webglyph has a feature to display the created hieroglyphs in a Ptolemaic font. Using this feature, we created another version of our test text.

Today, the majority of [JSesh](https://jsesh.qenherkhopeshef.org/) is used. If you follow our blog, you should be familiar with the name! There is an [online service](https://pure-sierra-27254.herokuapp.com/) that can generate JSesh hieroglyphs, cf. the repo <https://github.com/macleginn/jsesh-web>. Unfortunately, the application was down, so we didn't create a version with JSesh hieroglyphs.

Loyal readers of our blog know the name Nederhof. Mark-Jan Nederhof has developed [RES](https://mjn.host.cs.st-andrews.ac.uk/egyptian/res/), a hieroglyphic input system. There is also a [javascript based version](https://mjn.host.cs.st-andrews.ac.uk/egyptian/res/js/index.html). With this we have created a web page with the hieroglyphs of the test text. So we have an additional version of our test text.

So the text is available in five different images:

* [Original](https://commons.wikimedia.org/w/index.php?title=File:Egypte_louvre_272_stele.jpg&oldid=619070409)
* [Wikisource](/img/blog/wikisource_senusret.jpg)
* [Webglyph](/img/blog/winglyph_senusret.jpg)
* [Webglyph, Ptolemaic](/img/blog/winglyph_senusret_ptol.jpg)
* [RES](/img/blog/res_senusret.jpg)

The text consists of 65 hieroglyphs. We uploaded the five images into hieroglyphs.ai and marked the respective hieroglyphs. This was an interesting experience: If the characters are not centered properly, they may not be recognized correctly. In this respect it will be a bit difficult if you want to repeat our test. We summarize our results in the following table:

| image  | problems | recognition rate |
| ------ | -------- | ---------------- |
| original | P6 instead of U23<br />N5 instead of Aa1<br />T22 instead of M17<br />U33 instead of M17<br />N5 instead of Aa1<br />Y1 instead of N17<br />Aa11 instead of N17<br /> | 58/65 → 89 % |
| wikisource | W18 instead of W17<br />S43 instead of Z1<br />O28 instead of U23<br />S43 instead of Z1 | 61/65 → 94 % |
| winglyph | S43 instead of Z1<br />S43 instead of Z1<br />S43 instead of Z1<br />A40 instead of B1 | 61/65 → 94 % |
| winglyph, ptolemaic | O49 instead of Aa1<br />O49 instead of Aa1<br />O34 instead of N35 | 62/65 → 95 % |
| res | W18 instead of W17<br />S43 instead of R14<br />S43 instead of Z1<br />S43 instead of Z1<br />O34 instead of N35 | 60/65 → 92 % |

The recognition rates are really good. 95% means that only every twentieth hieroglyph is not recognized correctly. Also the original has almost 90 %. Congratulations to hieroglyphs.ai!

The problems can be classified quite well:

1. high narrow characters: This is especially difficult with the original. A special case is the stroke Z1, which caused problems almost everywhere.
2. circles: The recognition can badly distinguish 𓈒, 𓇳, 𓐍 and 𓊖. In fact, often there are only circles in the original, with no interior drawing. Without context information, correct recognition is not possible at all.

Do all texts now have such a high recognition rate? Unfortunately not! We have tested <https://www.metmuseum.org/art/collection/search/544346>. Here the recognition rate drops to 78%: S29 instead of M17, N33 instead of Aa1, N33 instead of Aa1, Y2 instead of O34, S29 instead of M17, S29 instead of M17, N33 instead of Aa1, T30 instead of I5. The results for the facsimiles of the early inscriptions from Helwan ([Köhler & Jones: Helwan II. The Early Dynastic and Old Kingdom Funerary Relief Slabs, 2009](https://aegyptiaca.uni-muenster.de/Record/111962)) are even worse. Therefore: Do not expect miracles! The software is no better than an Egyptologist with great experience who can deal with character variance, context, and partial destruction. The software can't do that (yet). But it does recognize standardized characters very well.

That's why we think that the biggest potential at the moment lies in retro-digitization. But for that to happen, the software has to be able to recognize not only individual characters, but also the flow of text. In other words, the next step is for the software to be able to find the lines on its own and then work through the individual characters one by one. There was once a mail in EEF about this, with the reference to:

> Andrea Barucci, Michela Amendola, Fabrizio Argenti, Chiara Canfailla, Costanza Cucci, Tommaso Guidi, Lorenzo Python, Massimiliano Franci, Discovering the ancient Egyptian hieroglyphs with Deep Learning. IFAC-Book Series, 2023. 127 pp. ISBN 978-88-947081-1-0. The free e-Book (PDF) can be downloaded from the IFAC-CNR website at <http://www.ifac.cnr.it/index.php>

In a [previous blog](https://oraec.github.io/2023/05/05/roadmap-and-preliminary-work-for-a-hieroglyphic-metasearch-engine.html) we briefly mentioned OCR for hieroglyphs. We were interested in the possibility of recognizing hieroglyphs from computer generated images for services like [Ramsès](http://ramses.ulg.ac.be/) or [VÉgA](https://www.vega-vocabulaire-egyptien-ancien.fr/). If hieroglyphs.ai develops in the direction mentioned above, this would be a good area of application.

Our conclusion is that this is a great thing. We are positively surprised how good the recognition is with computer generated hieroglyphs and partly with original hieroglyphs and hope that the development will continue!

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a></p>
