# MdC to Unicode converter

In this blog we present a small tool that allows you to convert hieroglyphs to Unicode: <https://oraec.github.io/corpus/mdc_to_unicode_converter.html>

![MdC to Unicode converter](/img/blog/mdc_to_unicode_converter.jpg "MdC to Unicode converter")

You remember, we published the [recommendations for encoding Egyptian hieroglyphs in Unicode](https://oraec.github.io/2022/09/28/recommendations-encoding-hieroglyphs.html) and converted quite a few freely available hieroglyphic encodings ([Wikisource](https://github.com/oraec/formerly-mdc-now_unicode/tree/main/wikisource), [MdC texts from JSesh](https://github.com/oraec/formerly-mdc-now_unicode/tree/main/jsesh), [AES](https://github.com/oraec/formerly-mdc-now_unicode/tree/main/AES)) to Unicode. The basis for the conversion is a [mapping](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/complete_mapping.csv) we published in [one of our Github repositories](https://github.com/oraec/formerly-mdc-now_unicode). This tool presented here allows to perform the conversion on the web. All no witchcraft, but very, very simple Javascript!

The web page consists of two textareas, a button and some text. If you enter hieroglyphic codes in the upper box and click the button, the hieroglyphs will be converted to Unicode and displayed in the lower box. We have filled the first box - quasi as an example - with hieroglyphic code. It is a well-known sentence from Sinuhe. See here: <https://oraec.github.io/corpus/oraec17-18.html> So you have an impression, which code you can enter there: Gardiner code, its phonetic values and the operators ``-``, ``*``, ``:`` and ``&`` known from [MdC](https://en.wikipedia.org/w/index.php?title=Manuel_de_Codage&oldid=1012543887). Furthermore, the tool can also handle parentheses, rotations, mirrorings and destruction specifications.

After clicking the button, the result is displayed in the box below. The Unicode hieroglyphs use the ligatures from the [EgyptianHiero](https://github.com/MKilani/Djehuty) font. As you can see from the example, some ligatures are unfortunately a little bit broken :-(

Have fun with the conversion!
