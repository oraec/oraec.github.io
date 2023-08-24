# Leiden Unified Transliteration

Hi folks! Recently, the [ICE](https://ice2023.com/) took place. What is the ICE? It's the largest Egyptological event that takes place every four to five years. This time Leiden was the venue, and about 800 Egyptologists attended. 15 of them met on August 8th to discuss transliteration. (It is a pity that Alexander Ilin-Tomich, Mark-Jan Nederhof and Serge Rosmorduc, some of whom were in Leiden, did not also participate. They could have strengthened the IT component. We will see below where the problem lies). At the end of the congress, the LUT, [Leiden Unified Transliteration](https://ice2023.com/en/news/lut), was adopted. What does transliteration mean? Hieroglyphs - contrary to popular belief - are not pictographic writing, but like our alphabets, represent spoken language. Hieroglyphs (at least many of them) have phonetic values, so that they have the function "phonogram". To reproduce the phonetic value of a sign, transliteration is used. A 𓅓 has the phonetic value m, so the transliteration m is used. A 𓐛 also has the phonetic value m, so m is transliterated here as well. A transliteration is therefore not a representation of the graphic system. It does not matter which sign with the phonetic value m is used, the transliteration writes an m to the same extent. A new transliteration sign is needed if - shortened - another sound is present. For the Old Kingdom, the two graphemes 𓊃 and 𓋴 represent two different phonemes, so - for the transliteration of the texts of the Old Kingdom - two transliteration signs are needed. In short, the transliteration reproduces the consonants written through the hieroglyphs without representing the peculiarities of the script with its determinatives, etc.

Egyptology has known the process of transliteration since the 19th century. What is so special about it that a major conference has to deal with it? Unfortunately, the transliteration of Egyptian is not uniform. Some write an s for the hieroglyph 𓋴, others a ś. Some write an ḳ for the hieroglyph 𓈎, some a q. This is very annoying in our digital age, because then you have four different options for the word 𓌟𓏤: qs, qś, ḳs, and ḳś. So if you search for this transliteration in a search engine of your choice, you have to enter four variants! In this respect, it would be nice if Egyptology had a standardized transliteration. This problem is compounded by the fact that Egyptology uses different signs for its transliteration. The Egyptological Alif appears as the correct ꜣ or as the incorrect ȝ, which is actually a Middle English sign.

For a better understanding of the differences, we have created a small table here that shows the special signs of the transliteration in different projects:

| Project  | 𓄿 | 𓇋 | 𓇌 | 𓈎 |
| ------------- |:-------------:|:-------------:|:-------------:|:-------------:|
| [AED](https://simondschweitzer.github.io/aed/index.html)      | ꜣ | j | y | q |
| [AGÉA](https://www.ifao.egnet.net/bases/agea/noms/)      | ȝ | ỉ | y | q |
| [IFAO Karnak Cachette](https://www.ifao.egnet.net/bases/cachette/)      | ȝ | j | y | q |
| [Karnak](http://sith.huma-num.fr/karnak)      | ȝ | j | y | q |
| [ORAEC](https://oraec.github.io/corpus)      | ꜣ | j | y | q |
| [PNM](https://pnm.uni-mainz.de/info)      | ꜣ | j | jj | q |
| [Ramsès](http://ramses.ulg.ac.be/)      | ꜣ | j | y | ḳ |
| [TLA](https://thesaurus-linguae-aegyptiae.de/)      | ꜣ | j | y | q |
| [Trismegistos](https://www.trismegistos.org/)      | ȝ | ỉ | y | q |
| [TSL](https://thotsignlist.org/) | A | j | y | q |
| [VÉgA](https://www.vega-vocabulaire-egyptien-ancien.fr/)      | ȝ | j | y | q |
| [Wikisource](https://wikisource.org/wiki/Main_Page/Ancient_Egyptian)      | 3 | j | y | ḳ |

The table nicely shows the inconsistency, which is on two levels: First, different signs are used for a hieroglyph, i.e. y or jj or q or ḳ. Second, different Unicode signs are used for one sign, i.e., [ꜣ](https://graphemica.com/%EA%9C%A3), [ȝ](https://graphemica.com/%C8%9D), [A](https://graphemica.com/A), and [3](https://graphemica.com/3) for 𓄿. The [ỉ](https://graphemica.com/%E1%BB%89) for 𓇋 is not even listed as a possibility for the Egyptological Yod at [Rosmorduc's overview](https://github.com/rosmord/mac_transliteration_keyboards#egyptological-yod)!

Let's see what LUT proposes. LUT has a total of 26 transcription signs, which looks broadly traditional. It does not follow Rößler's system, which Schenkel introduced in Egyptology. Nor does it adopt Schneider's suggestions, which, if we survey it correctly, did not find favor either. (On those systems, see <https://en.wikipedia.org/w/index.php?title=Transliteration_of_Ancient_Egyptian&oldid=1170366739>) It is a little surprising that Joachim Quack, as convenor of the meeting that decided LUT, agreed to these transcription marks; for he uses Schenkel's system exclusively. So, LUT says, no ṭ, č̣ and č, but d, ḏ and ṯ! At the moment, we can only speculate about the motivations. Probably, LUT was meant to incorporate elements that many Egyptologists use. Schenkel's system is not very well received, so LUT without Schenkel's signs is more likely to gain acceptance. Perhaps the degree of diffusion is also the key reason for using q rather than ḳ. As we have seen above, most projects use q. There are possibly two other factors at play. First, especially for beginners, there is a risk of confusion between k and ḳ. Writing q avoids this problem. Second, on the computer, a q can be typed directly. A ḳ, on the other hand, is more difficult to generate. But these are only speculations concerning the motivation. Let's go back to the signs! That a š is used for 𓈙 is not surprising. We limit ourselves to four cases: 𓎤, 𓄿, 𓇋 and 𓏭, which we want to discuss.

## 𓎤

[Peust, Egyptian Phonology](https://aegyptiaca.uni-muenster.de/Record/14920), pp. 107 ff. discusses the possibility that Egyptian has seven different velars. Thus, in the Old Kingdom, the grapheme 𓎤 could represent the phoneme k<sub>2</sub><sup>w</sup>. Usually 𓎤 is transliterated as g, so LUT also suggests it. One could consider choosing a separate sign for 𓎤. If you are wondering why we are even considering 𓎤: Well, LUT has its own transliteration sign for 𓏭 too!

## 𓄿

For the LUT there is a [PDF](https://ice2023.com/cache/leiden-unified-transliterationtranscription-12-aug.1963/leiden-unified-transliterationtranscription-12-aug.pdf) where you can see the codes of the transliteration signs. Hooray! The LUT takes the correct ꜣ for the Egyptological Alif! This is an important statement. We saw the big mess at the top of the table. Hopefully the correct sign will prevail.

## 𓇋

Unlike 𓈎, the LUT does not suggest the j that most projects use. The LUT thus takes the typographically more difficult route, since the chosen sign is not as easy to produce as j. However, the real problem lies elsewhere and is comparable to the current situation with ꜣ. As [Alexander Ilin-Tomich](https://pnm.uni-mainz.de/tools/unicode/#popup2) points out, completely different Unicode signs are used for the alternative sign to j. There are i̓, i͗, and i҆, which modify the normal i in three different ways. In addition to i as the base, the dotless ı is also used. So there are three more possibilities: ı̓, ı͗, and ı҆. These are not just potential cases, but several of these variants are actually used and recommended, as [Alexander Ilin-Tomich](https://pnm.uni-mainz.de/tools/unicode/#popup2) compiles. As of 2019, there is a separate sign in Unicode for the Egyptological Yod: ꞽ. Unfortunately, this sign is not yet implemented in many fonts, so again, the sign is not properly visible. The digital projects mentioned above that do not use j do not choose any of the previous seven possibilities, but [ỉ](https://graphemica.com/%E1%BB%89). The LUT introduces another sign: In the PDF of transliteration signs, there is a [ἰ](https://graphemica.com/%E1%BC%B0), which actually belongs to the Greek alphabet. Dear readers, have you lost the overview? We can well understand that. This is also our great concern. At the moment we already have the ꜣ catastrophe when different Unicode signs are used for the Egyptological Alif. There is a great danger that the rejection of the unambiguous j will create another transliteration disaster, namely many different variants for the 𓇋. It is not our place to criticize the rejection of the j. We simply point out that it unnecessarily creates problems in the digital world.

## 𓏭

Surprisingly, 𓏭 gets its own transcription sign; i.e. there are three separate transcription signs for the three hieroglyphs 𓇋, 𓇌 and 𓏭. This is very unusual. All the above projects have only two transliteration signs for these three hieroglyphs. Two signs are used because the two graphemes 𓇋 and 𓇌 represent two different phonemes in the rendering of Semitic words, cf. [Albright, Vocalization](https://aegyptiaca.uni-muenster.de/Record/80502), p. 34. So where does the third sign come from? Peust, Egyptian Phonology, pp. 49 f. wants to differentiate between the three signs in transliteration. He writes about the distribution of the hieroglyphs:

> In Middle Egyptian all three signs indicated are in current use and variation among them becomes rare. It can be roughly stated that at this time 𓇋 is not restricted in distribution, whereas 𓇌 can appear at a morpheme boundary only, and 𓏭 is even more restricted in that it is used only morpheme-finally.

Thus, according to Peust, the distribution is done for morphemic and not for phonematic reasons. He writes further on the function:

> At least as can be judged from Coptic, there seems to have no phonetic difference between 𓇋, 𓇌, and 𓏭. The sounds rendered by all three signs are equally preserved as /j/ or lost by the same conditions in Coptic. It is possible that these signs never expressed a phonetic distinction but instead their functional difference basically was to indicate morphological boundaries or other features. It is also possible that they did originally express a phonetic distinction which was lost later.

So there is no evidence for a phonological difference. But this is exactly what is needed to postulate an independent transliteration sign! All that remains is the assertion that Middle Egyptian seldom exchanged the three signs. According to this, the three transliteration signs are exclusively peculiarities of the graphic system. But even this does not seem to be true. With our [metasearch engine](https://oraec.github.io/corpus/search/search_hieroglyphs.html) it is very easy to find spellings with 𓏭. The data from the PNM project speak for themselves. (We stopped our survey after twenty hits, because we think the results are already clear).

| Name | Some spellings |
| ---- | -------------- |
| [jtjj](https://pnm.uni-mainz.de/name/66) | 𓇋𓀁𓍘𓇋, 𓇋𓀁𓍘𓇌, 𓇋𓏏𓏭 |
| [jṯꜣ.j](https://pnm.uni-mainz.de/name/2406) | 𓇋𓅷𓄿𓇋, 𓇋𓅷𓄿𓏭 |
| [nmt.j](https://pnm.uni-mainz.de/name/721) | 𓌰𓅓𓏏𓏭, 𓈖𓌰𓅓𓏏𓇋, 𓈖𓌰𓅓𓏏𓇌 |
| [rns.j](https://pnm.uni-mainz.de/name/25) | 𓂋𓈖𓋴𓇋, 𓂋𓈖𓋴𓇌, 𓂋𓈖𓋴𓏭 |
| [ḫnt.j-ẖt.jj-ḥtp](https://pnm.uni-mainz.de/name/291) | 𓏃𓈖𓏏𓄡𓍘𓇌𓊵𓏏𓊪, 𓏃𓈖𓏏𓄡𓏏𓏭𓊵𓏏𓊪, 𓏃𓄡𓍘𓇋𓊵𓏏𓊪 |
| [snb.tj⸗sj](https://pnm.uni-mainz.de/name/216) | 𓋴𓈖𓃀𓏏𓋴𓏭, 𓋴𓈖𓃀𓍘𓋴, 𓋴𓈖𓃀𓏛𓏏𓋴𓇋 |
| [kjj](https://pnm.uni-mainz.de/name/798) | 𓎡𓇌, 𓎡𓏭, 𓎡𓇋 |

The three hieroglyphs are interchangeable in the personal names! It seems to us a suitable topic for a final thesis to investigate the distribution of 𓇋, 𓇌, and 𓏭. A working hypothesis would be that the regularity of the distribution depends on genre and register and is purely graphemic. Substantial evidence that a third phoneme is represented in 𓏭, requiring a separate transliteration mark, does not seem to exist.

Therefore, in our opinion, a separate ï is not recommended. In addition, we would like to point out that adapting the data is very time-consuming, since it cannot be done automatically. Do you really want to go to all that effort just because of a questionable sign distribution without any phonemic reference? Sorry, no thanks, we cannot follow this suggestion.

## Standardization

The above points have been lost in detail; in general it is a laudable view that Egyptology treats the same things in the same way, i.e. that one agrees on a uniform system. But we still see two general problems here:

Standardization prescribes the status quo. It is difficult to incorporate new findings into a standardized system. Transliteration signs already do not reflect the state of phonological research. 𓂧 is considered by many to be an emphatic sound. Accordingly, a ṭ is a much better rendering than a d, which can lead those unfamiliar with the subject to make incorrect etymological equations.

We have described above the problem that to search for 𓌟𓏤 one has to enter four variants into the search engine. But these are regular equivalents. Much worse are the cases where the Egyptological transliteration offers variants that cannot be handled in a regular way. The scribe is sš or zẖꜣ, the sealer ḫtm.tj or sḏꜣw.tj, the sun god Rꜥ or Rꜥw, the head tp or dp, "to be ill" mr or mḥr, and the king nzw, nswt, or njswt. This is the real problem with transliteration searches in a search engine. You are dealing with an unpredictable variance.

So this time we conclude rather pessimistically. True, it would be nice to have a uniform system. We can certainly talk about the details mentioned above. But such variants as ḥtp dj nswt, ḥtp-ḏ-nzw or ḥtp ḏi̯ njswt are the real problem.

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a></p>
