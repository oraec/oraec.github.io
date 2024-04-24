# New Unicode Texts

Hi folks. As you know, our focus is on Unicode. Our first blogs were about converting reusable digital data of Egyptian texts to Unicode and publishing [recommendations](https://oraec.github.io/2022/09/28/recommendations-encoding-hieroglyphs.html) for using Unicode hieroglyphs. Among other things, we took the [great repository of JSesh texts](https://github.com/rosmord/MDC-texts) and [converted](https://oraec.github.io/2022/10/10/missing-unicode-characters-and-further-mapping-problems.html) them to Unicode. In the meantime, a lot has happened in this repository: new texts have been added and existing texts have been licensed under a free license. So we decided to update it. In this blog we explain the results:

The repository [formerly-mdc-now_unicode](https://github.com/oraec/formerly-mdc-now_unicode) now contains 16 new texts, namely:

* [Abydos, grande inscription dedicatoire](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/Abydos%2C%20grande%20inscription%20dedicatoire.md)
* [Book of the dead Chapter 17](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/Book%20of%20the%20dead%20Chapter%2017.md)
* [P_Harris_I_Discours aux dieux, Thebes](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/P_Harris_I_Discours%20aux%20dieux%2C%20Thebes.md)
* [P_Harris_I_Introduction](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/P_Harris_I_Introduction.md)
* [P_Harris_I_Thebes, Liste A](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/P_Harris_I_Thebes%2C%20Liste%20A.md)
* [P_Harris_I_Thebes, Liste B](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/P_Harris_I_Thebes%2C%20Liste%20B.md)
* [P_Harris_I_Thebes, Liste C](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/P_Harris_I_Thebes%2C%20Liste%20C.md)
* [P_Harris_I_Thebes, Liste D](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/P_Harris_I_Thebes%2C%20Liste%20D.md)
* [P_Harris_I_Thebes, Liste E](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/P_Harris_I_Thebes%2C%20Liste%20E.md)
* [P_Harris_I_Thebes, Liste F](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/P_Harris_I_Thebes%2C%20Liste%20F.md)
* [P_Harris_I_Vignette Thebes, pl](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/P_Harris_I_Vignette%20Thebes%2C%20pl.md)
* [P. Prisse (Gemnikai and Ptahotep)](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/P.%20Prisse%20(Gemnikai%20and%20Ptahotep).md)
* [Qadesh Poem-Pentaour](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/Qadesh%20Poem-Pentaour.md)
* [Sinuhe](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/Sinuhe.md)
* [Stela Cairo CGC 34025-Israel Stela](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/Stela%20Cairo%20CGC%2034025-Israel%20Stela.md)
* [Stela Serabit el Khadim Sobekherheb](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/Stela%20Serabit%20el%20Khadim%20Sobekherheb.md)

We would like to thank the authors Kaan Eraslan, Émil Joubert, R. Monfort, S. Rosmorduc for encoding the new data and Serge Rosmorduc for publishing it in the reusable repository.

As expected, the MdC data of these texts contain a number of encodings that we have not yet encountered in the transformation to Unicode, such as O42C or W17D. In most cases, these are variants. However, according to Unicode principles and our recommendations, the actual characters should be encoded. Accordingly, we have extended our mapping so that an O42C is converted to 𓊏.

In addition, there are some codes that represent characters that cannot yet be represented in Unicode. We had already compiled [some characters](https://oraec.github.io/2022/10/10/missing-unicode-characters-and-further-mapping-problems.html#missing-unicode-characters) in our transformation at that time. We offer here the cases of missing Unicode characters resulting from this transformation:

## Missing Unicode characters

### A82

* semantic value: to throw
* source: [KRI IV](https://archive.org/details/KennethA.KitchenRamessideInscriptionsVol4), 14.8.

### B75

* semantic value: female captive
* source: [KRI II](https://archive.org/details/KennethA.KitchenRamessideInscriptionsVol2), 93.8.

### D283

* phonetic value: js
* semantic value: testicles
* source: [Leitz, Christian: Quellentexte zur Ägyptischen Religion I. Die Tempelinschriften der griechisch-römischen Zeit. 2004, p. 158](https://aegyptiaca.uni-muenster.de/Record/37259).

### E80

* phonetic value: ḫḫ
* semantic value: griffin
* source: [Cauville, Sylvie: Dendara. Le fonds hiéroglyphique au temps de Cléopâtre. 2001, p. 77](https://aegyptiaca.uni-muenster.de/Record/29959) & [KRI II](https://archive.org/details/KennethA.KitchenRamessideInscriptionsVol2), 55.1-4.
* variant: E80A

### E100

* phonetic value: nb
* semantic value: cow
* source: [Cauville, Sylvie: Dendara. Le fonds hiéroglyphique au temps de Cléopâtre. 2001, p. 79](https://aegyptiaca.uni-muenster.de/Record/29959).
* variants: E100A,E100C

### G106

* semantic value: Harsomtus
* source: [Cauville, Sylvie: Dendara. Le fonds hiéroglyphique au temps de Cléopâtre. 2001, p. 113](https://aegyptiaca.uni-muenster.de/Record/29959).

### N6B

* phonetic value: nzw-bjt
* source: [Cauville, Sylvie: Dendara. Le fonds hiéroglyphique au temps de Cléopâtre. 2001, p. 150](https://aegyptiaca.uni-muenster.de/Record/29959).

### O137

* phonetic value: bḫn
* source: [Leitz, Christian: Quellentexte zur Ägyptischen Religion I. Die Tempelinschriften der griechisch-römischen Zeit. 2004, p. 168](https://aegyptiaca.uni-muenster.de/Record/37259).

### R31A

* semantic value: socle
* source: [Cauville, Sylvie: Dendara. Le fonds hiéroglyphique au temps de Cléopâtre. 2001, p. 189](https://aegyptiaca.uni-muenster.de/Record/29959).

### R42

* phonetic value: sḥtp,snṯr
* source: [Cauville, Sylvie: Dendara. Le fonds hiéroglyphique au temps de Cléopâtre. 2001, p. 189](https://aegyptiaca.uni-muenster.de/Record/29959).

### Aa56

* phonetic value: m
* source: [Cauville, Sylvie: Dendara. Le fonds hiéroglyphique au temps de Cléopâtre. 2001, p. 252](https://aegyptiaca.uni-muenster.de/Record/29959).
* please note that this sign is not identical with F45A

It seems promising to go through the work of Cauville and Leitz regarding missing Unicode hieroglyphs.

In any case, we have also added the new variants and the placeholders for the missing characters to our [MdC converter](https://oraec.github.io/corpus/mdc_to_unicode_converter.html) so that you can correctly convert a "W17D-n:t*y-iwn-nfr" to 𓏃𓈖𓏏𓏭𓉺𓄤 on the web.

Back to the new texts! These are also accessible via [our metasearch engine for hieroglyphs](https://oraec.github.io/corpus/search/search_hieroglyphs.html). So if you search for the phrase 𓌞𓋴𓂻𓎟𓀀𓆑, you will see that it is used in Sinuhe.

See you next time!

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a></p>
