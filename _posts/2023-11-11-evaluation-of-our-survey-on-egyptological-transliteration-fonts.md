# Evaluation of our survey on Egyptological transliteration fonts

## Introduction

The [ICE](https://ice2023.com/) took place this summer. An important event of this congress has been dominating the news ever since: The [Leiden Unified Transliteration](https://ice2023.com/en/news/lut) was adopted, which is intended to standardize the transliteration of Egyptian. In an earlier [blog](https://oraec.github.io/2023/08/24/leiden-unified-transliteration.html) we discussed this in detail. The Leiden Unified Transliteration focuses on which signs should be used, e.g. q instead of ḳ. However, the Leiden Unified Transliteration does not deal with the conversion of individual characters to Unicode. The Leiden Unified Transliteration PDF writes [ἰ](https://graphemica.com/%E1%BC%B0) for 𓇋. However, the character belongs to the Greek alphabet. As we have listed in our [blog](https://oraec.github.io/2023/08/24/leiden-unified-transliteration.html), there are several solutions for displaying the transliteration sign for 𓇋 in Unicode. Even if Egyptology were to stop writing j for 𓇋, there would be very different implementation strategies in circulation, which would run counter to the idea of standardization.

This problem is exacerbated by the fact that non-Unicode fonts are also used in Egyptology. So there are not only different variants of what the transliteration sign for 𓇋 should look like. These fonts only convert regular signs like i or A into transliteration signs. You can imagine the chaos this creates in the digital world, can't you? What can be done about it? Beside the good old [Transliteration to Unicode Converter](https://pnm.uni-mainz.de/tools/unicode/), there are currently two new solutions:

1. Fabian Wespi has created an [add-on for Word](https://github.com/fwespi/fwespi.github.io) that converts the transliteration of non-Unicode fonts to Unicode.
2. Alexander Ilin-Tomich has developed [a Python library](https://github.com/ailintom/umschriftpy) that converts non-Unicode transliterations to Unicode.

Thank you so much for this! That's great! But how big is the audience for these solutions? How many Egyptologists are still using non-Unicode fonts? To find out, we launched a [survey](https://oraec.github.io/2023/10/12/survey-egyptological-transliteration-fonts.html) a month ago. We asked you what transliteration font you use, how old you are, and what region you are from. After we announced our survey on [EEF](https://www.egyptologyforum.org/EEFNEWS.html), the number of participants increased. In total, 108 people participated in the survey. Thank you very much for that! That's very nice!

Before we get into the details, let's start with a disclaimer: this survey does not meet any scientific standards. To name just a few problems:

* The data is not (necessarily) representative. Look at the distribution of regions, for example.
* The survey does not control how reliable the data collection is. Anyone can vote multiple times and lie about their age.
* Further conclusions are not possible due to the small data base.

The survey provides some general expectations about whether non-Unicode fonts are being used and, if so, who is using them. As we will see, they are really quite general.

## Evaluation

### In general

The general distribution is - at least for us - very surprising. Out of 108 people, 74 use a non-Unicode font! That's almost 70 percent! So less than a third of the participants use a Unicode font. (Sarcastic remark from us: we are in the year 2023!). Here is a tabular overview:

| Font | Number | Percentage |
| ---- | ------ | ---------- |
| non-Unicode | 74 | 68.5 % |
| Unicode | 34 | 31.5 % |

We also visualized the data very simply with a barplot in R:

![Font Distribution](/img/blog/font_distribution_complete.jpeg "Font Distribution")

So for those of you in a hurry: Egyptology continues to use non-Unicode fonts. Updates of such fonts will still find enough users today. The solutions presented above have a large target group.

### Non-Unicode fonts

Most participants who use a non-Unicode font use TrlitCG Times. At 43, this number is even higher than the number of all those using a Unicode font! Just under a quarter of all participants use the Transliteration font. TranscriptionTTn is used by 4 people, 2 use another non-Unicode font.

Here again a barplot:

![Non-Unicode Font Distribution](/img/blog/font_distribution_nonunicode.jpeg "Non-Unicode Font Distribution")

### Unicode fonts

Unlike non-Unicode fonts, we could not anticipate their use in our selection. Most of the people who use such fonts use a font other than the one in our selection. This is 20 people in total. In addition, 7 people use New Athena, 5 people use Gentium, and only 2 people use our favorite Charis SIL.

This is the last time we will announce a barplot. From now on it will follow directly.

![Unicode Font Distribution](/img/blog/font_distribution_unicode.jpeg "Unicode Font Distribution")

### Age

We had previously hypothesized that the non-Unicode fonts were mainly used by older colleagues because they had been using the fonts for 20 years. We also assumed that the digital natives would rely on Unicode. First, the age distribution of the participants:

![Age Distribution](/img/blog/age_distribution.jpeg "Age Distribution")

So we had predetermined decades. Most of the participants are between 26 and 45 years old. Now let's look at the distribution of fonts per age segment:

![Font Distribution Age under 26](/img/blog/font_distribution_under_26.jpeg "Font Distribution Age under 26")

![Font Distribution Age 26-35](/img/blog/font_distribution_26_35.jpeg "Font Distribution Age 26-35")

![Font Distribution Age 36-45](/img/blog/font_distribution_36_45.jpeg "Font Distribution Age 36-45")

![Font Distribution Age 46-55](/img/blog/font_distribution_46_55.jpeg "Font Distribution Age 46-55")

![Font Distribution Age 56-65](/img/blog/font_distribution_56_65.jpeg "Font Distribution Age 56-65")

![Font Distribution Age over 65](/img/blog/font_distribution_over_65.jpeg "Font Distribution Age over 65")

Non-Unicode fonts are ahead in all segments. In the age segment between 36 and 45, the distribution is almost even. Otherwise, the gap is quite large. Our hypothesis "The younger, the more Unicode" is not confirmed by the data.

### Region

We mentioned above that the data is not representative. This is clearly shown here. Only a tiny fraction of the many Egyptian Egyptologists participated in this survey. The distribution by origin is as follows:

![Region Distribution](/img/blog/region_distribution.jpeg "Region Distribution")

So most of the participants come from Europe! Now the distribution of the fonts by region:

![Font Distribution Africa](/img/blog/font_distribution_africa.jpeg "Font Distribution Africa")

![Font Distribution Asia](/img/blog/font_distribution_asia.jpeg "Font Distribution Asia")

![Font Distribution Australia & Oceania](/img/blog/font_distribution_australia_oceania.jpeg "Font Distribution Australia & Oceania")

![Font Distribution Europe](/img/blog/font_distribution_europe.jpeg "Font Distribution Europe")

![Font Distribution North America](/img/blog/font_distribution_northamerica.jpeg "Font Distribution North America")

![Font Distribution South America](/img/blog/font_distribution_southamerica.jpeg "Font Distribution South America")

Again, you can see the popularity of non-Unicode fonts. Only in Australia & Oceania is the number equal. But with only 6 participants from this region, it is difficult to extrapolate anything.

### Conclusion

Most Egyptologists today still use the proven non-Unicode fonts. If you want to ensure the interchangeability of Egyptological data, you cannot currently rely on the end user. Instead, publishers and digital services must convert the data created by Egyptologists into sustainable Unicode data. Sobering, but that's the reality!

## Data

| Unicode? | font | region | age |
| -------- | ---- | ------ | --- |
| non-Unicode | another non-Unicode font | North America | > 65 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 26-35 |
| Unicode | another Unicode font | Europe | 36-45 |
| Unicode | another Unicode font | Europe | 26-35 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 36-45 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 26-35 |
| Unicode | another Unicode font | Europe | 26-35 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 56-65 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 26-35 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 26-35 |
| non-Unicode | Transliteration (non-Unicode) | Africa | 26-35 |
| non-Unicode | TrlitCG Times (non-Unicode) | Australia & Oceania | > 65 |
| Unicode | another Unicode font | Europe | 36-45 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 56-65 |
| Unicode | another Unicode font | North America | > 65 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | < 26 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 46-55 |
| Unicode | another Unicode font | North America | > 65 |
| Unicode | another Unicode font | Australia & Oceania | 36-45 |
| non-Unicode | Transliteration (non-Unicode) | Asia | 56-65 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 46-55 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 26-35 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 46-55 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 56-65 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 26-35 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 56-65 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | < 26 |
| non-Unicode | TrlitCG Times (non-Unicode) | Africa | 26-35 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 56-65 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 26-35 |
| Unicode | another Unicode font | Europe | 36-45 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 26-35 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 36-45 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 46-55 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 36-45 |
| non-Unicode | Transliteration (non-Unicode) | North America | 46-55 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | > 65 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 56-65 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 26-35 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 36-45 |
| Unicode | Gentium (Unicode) | Europe | 26-35 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 36-45 |
| non-Unicode | UmschriftTTn (non-Unicode) | Europe | > 65 |
| Unicode | New Athena Unicode (Unicode) | Europe | 36-45 |
| Unicode | New Athena Unicode (Unicode) | Europe | 36-45 |
| Unicode | New Athena Unicode (Unicode) | Europe | 36-45 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 26-35 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 26-35 |
| non-Unicode | UmschriftTTn (non-Unicode) | Europe | 26-35 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 36-45 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | < 26 |
| Unicode | another Unicode font | Europe | 26-35 |
| non-Unicode | UmschriftTTn (non-Unicode) | Europe | 36-45 |
| Unicode | another Unicode font | Europe | 56-65 |
| Unicode | another Unicode font | Europe | 36-45 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 36-45 |
| Unicode | another Unicode font | Europe | > 65 |
| Unicode | another Unicode font | Europe | 26-35 |
| Unicode | Charis SIL (Unicode) | Europe | 36-45 |
| non-Unicode | TrlitCG Times (non-Unicode) | North America | 26-35 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 36-45 |
| Unicode | Gentium (Unicode) | North America | 36-45 |
| Unicode | Gentium (Unicode) | North America | 36-45 |
| non-Unicode | TrlitCG Times (non-Unicode) | North America | 26-35 |
| non-Unicode | Transliteration (non-Unicode) | Australia & Oceania | < 26 |
| non-Unicode | Transliteration (non-Unicode) | South America | 36-45 |
| Unicode | Charis SIL (Unicode) | Australia & Oceania | 26-35 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 36-45 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 26-35 |
| Unicode | New Athena Unicode (Unicode) | Europe | 26-35 |
| non-Unicode | another non-Unicode font | North America | > 65 |
| non-Unicode | TrlitCG Times (non-Unicode) | Australia & Oceania | 56-65 |
| Unicode | Gentium (Unicode) | Europe | > 65 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 36-45 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 46-55 |
| Unicode | Gentium (Unicode) | North America | 36-45 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | < 26 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 56-65 |
| Unicode | another Unicode font | North America | 56-65 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 36-45 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | > 65 |
| non-Unicode | TrlitCG Times (non-Unicode) | South America | 26-35 |
| Unicode | another Unicode font | Australia & Oceania | 56-65 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 56-65 |
| non-Unicode | TrlitCG Times (non-Unicode) | North America | 26-35 |
| non-Unicode | TrlitCG Times (non-Unicode) | North America | > 65 |
| Unicode | New Athena Unicode (Unicode) | North America | 46-55 |
| non-Unicode | TrlitCG Times (non-Unicode) | North America | > 65 |
| non-Unicode | TrlitCG Times (non-Unicode) | North America | 26-35 |
| Unicode | another Unicode font | Europe | 36-45 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 36-45 |
| Unicode | another Unicode font | Europe | 26-35 |
| non-Unicode | TrlitCG Times (non-Unicode) | North America | 26-35 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 56-65 |
| non-Unicode | TrlitCG Times (non-Unicode) | Asia | 26-35 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | > 65 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 56-65 |
| non-Unicode | Transliteration (non-Unicode) | South America | 56-65 |
| non-Unicode | UmschriftTTn (non-Unicode) | Europe | 36-45 |
| Unicode | another Unicode font | Europe | 26-35 |
| Unicode | New Athena Unicode (Unicode) | Europe | 36-45 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 26-35 |
| Unicode | New Athena Unicode (Unicode) | Europe | 26-35 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 26-35 |
| Unicode | another Unicode font | Europe | 36-45 |
| non-Unicode | TrlitCG Times (non-Unicode) | Europe | 26-35 |
| non-Unicode | Transliteration (non-Unicode) | Europe | 36-45 |
| Unicode | another Unicode font | North America | 56-65 |

## License

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a></p>
