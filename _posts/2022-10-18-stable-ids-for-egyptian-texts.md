# Stable IDs for Egyptian texts

In our last [blog](https://oraec.github.io/2022/10/14/four-challenges-when-converting-aes.html), we reported on the difficulty of converting [AES](https://github.com/simondschweitzer/aes) annotations to Unicode. What to do with those weird text names like `ZEEXFUQWKNA2LNL5VYYMHCBTCY` or `3QLY4N4MXJHYTFS5TVAIOJEN5Q`? Nobody can remember them!

Instead, we propose to introduce a system of stable IDs for Egyptian texts. Such a procedure is nothing unusual in Egyptology. For example, there is already a sequential numbering of all inscriptions of the early period, cf. Sperveslage, Gunnar: *Die frühen Inschriften Ägyptens. Eine Konkordanz der Nummerierungssysteme*. 2021.

The texts of the temples from the Greco-Roman period are recorded with numbers, cf. <http://www.tempeltexte.uni-tuebingen.de/portal/#/main>

The best known is the numbering system of [Trismegistos](https://www.trismegistos.org/). Here, too, there are consecutive numbers.

Now it would be easiest if we could reuse these systems to number the AES texts. But the majority of the texts are not recorded in the mentioned systems. Moreover, there are conceptual differences. For example, Trismegistos speaks of 'TM Texts', but in reality these elements are objects. The papyrus pNew York MMA 35.9.21 contains different texts. AES lists six different ones:

* `ADO4HPZ7DNBFPOKZ4AGZWM45HM` (1st Great Decree issued concerning the Gau of Igeret).
* `JTXNVXIX5FDTFLMHDD2EWC5CVI` (2nd Ritual of the Transfiguration of Osiris (Book IV))
* `UOCH377L6ZAODLJNW46P2ZXS2A` (3. The Revelations of the Secrets of the Four Spheres of Clay)
* `ZFYMIVEFZ5DI5LOBNAWGMVMFDM` (4. "Fall on your face" (ritual for the protection of the Neschmet bark))
* `TT3YCFBGXBEWREWYTEGUP3YU6Y` (5. Introduction of the crowd on the last day of the month of Tech (=Thot))
* `DS3MPLHGBJHPZIZPE3NPHGTN34` (6. Ritual of bringing out Sokar from the Shetait sanctuary).

Trismegistos, however, has only one number which stands for the entire papyrus: <https://www.trismegistos.org/text/57080>. From a text-linguistic point of view, the object-oriented approach advocated by Trismegistos, which has quite different emphases, is not to be recommended. One cannot lump six different texts together!

That's why we had to develop our own system to give all AES texts a memorable name. Our numbering is based on the relevance of the texts. O.k., one can argue about which text is more relevant than another. How should one measure something like that? We have chosen a very pragmatic approach:

All AES texts are also coded TEI-XML compliant, as so-called [AED-TEI](https://github.com/simondschweitzer/aed-tei). AED stands for the [Ancient Egyptian Dictionary](https://simondschweitzer.github.io/aed/). This dictionary offers not only translations, but also occurrences for the lexical entries. These occurrences are taken from the texts that are coded in AED-TEI. Our pragmatic approach is: The more often a text is used in AED, the more relevant the text is. The frequency determines the relevance! The most frequently used text in AED is the Piye inscription, so we start our count with this text. This is now [oraec1](https://oraec.github.io/corpus/oraec1.html). In second place is Mythes et Légendes du Delta. This is then our number 2, that is, [oraec2](https://oraec.github.io/corpus/oraec1.html). Following this principle, we assign a number to all AES texts. An 'oraec21', the ID for the Admonitions, is easier to remember than 'GJA5VMSJDFAOPG6TP6ZYY3KCRI', isn't it? You can find the complete list of the stable IDs [here](https://oraec.github.io/corpus/oraec_text_list.html).

To give you an idea of these IDs, we have created a separate page for each ID, which contains the metadata of this text, i.e. dating, location, etc. The CSS is very, very simple. It is based on the CSS of AED. The metadata itself are in turn links to their own pages. There you have the overview of all texts that belong to a certain metadate (is that how you say it?): [all texts from the time of Cheops](https://oraec.github.io/corpus/IS52YO4UPBG6ZO5BFFVWJ26OWY.html), [all texts from the Phoebe Apperson Hearst Museum of Anthropology](https://oraec.github.io/corpus/BZDESZAD7RELZJMBJ76ZMLSSUU.html), etc. An [overview](https://oraec.github.io/corpus/controlled_vocab.html) lists all entries of the controlled vocabulary. We use the controlled vocabulary from the [AED](https://github.com/simondschweitzer/aed-tei/blob/master/files/thesaurus.xml) for this purpose.

After all, we introduced the stable IDs only because of the conversion of hieroglyphs to Unicode. We did not forget that in all this work! For the AES texts we have created a folder in our [repository](https://github.com/oraec/formerly-mdc-now_unicode): <https://github.com/oraec/formerly-mdc-now_unicode/tree/main/AES> In addition, the pages with the stable IDs and their metadata have links to the corresponding hieroglyphics page.

Have fun browsing!
