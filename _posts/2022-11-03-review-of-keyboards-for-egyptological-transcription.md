# Review of keyboards for Egyptological transcription

## Introduction

Recently there was a post in the AKU blog: [Unicode ist keine Schriftart. Zur Problematik ägyptologischer Umschriftfonts](https://aku.hypotheses.org/3063). It's a very informative overview. Read it through! Use the Google translator if necessary!

Before Unicode, fonts were used to generate the Egyptological transcription characters that did not exist on the ASCII keyboard. As the post impressively shows, you can't search for a special transcription character then, because depending on the font a different key was used to generate this character. Thus, the data containing Egyptological transcription was not interchangeable. It must have been nerve-wracking to submit an article to a journal. Are all the transcription characters represented correctly? Or has my ḥ perhaps become an ḫ?

Searchability and interchangeability: these are two things that should actually work with the use of Unicode. However, the blogpost points out that there are problems here as well. Namely, Egyptology uses two different variants of aleph: (the correct) ꜣ and (the incorrect) Ȝ. The Ȝ is actually a character of a Middle English letter. The IFAO has chosen this character only because of the external similarity. And because of the importance of the IFAO, some have adopted the Ȝ, such as [Trismegistos](https://www.trismegistos.org/) or [Egyptomaniak](http://www.egyptomaniak.gr/Egyptian%20Texts.htm).

Now, if you want to search for pꜣ on the Internet, you have to search twice, once for pꜣ and once for pȜ! This is - there is nothing to gloss over - disastrous. We should all follow the call of [Serge Rosmorduc](https://github.com/rosmord/mac_transliteration_keyboards/#why-no-ifao-compatible-keyboard), quoted by the AKU post:

> We now have alph, ayin, and yod in Unicode, let's use them.

How to enter Egyptological transcription characters on the computer? We do not consider mobile systems here and do not go into [SwiftKey](https://en.wikipedia.org/w/index.php?title=Microsoft_SwiftKey&oldid=1116163978) or the like. We limit ourselves only to desktop computers. There you can use not only your standard input keyboard, which produces an ``n`` for each press on the ``n`` key. You can also use other keyboard layouts that produce something completely different when you press ``n``, say ``ⲛ``. So there are also keyboards for Egyptological transcription. Let's take a look at those in this blogpost! (Pretty long preface, isn't it?).

What must such a keyboard be able to do? If it doesn't use the correct alef, it promotes the mess of encodings described above. Anything that perpetuates this disaster should not be used. Decisive criterion in the evaluation is thus the use of the correct alef, the correct ayin and the correct yod. The correct yod is only available from [Unicode 12](https://unicode.org/versions/Unicode12.0.0/), which was published in 2019. So no keyboard older than 2019 (or last updated before 2019) should be used!

What else? What are other important criteria? Are all characters available? So also i̯, ʾ and the capital letters? Is the keyboard user-friendly? It would be less user-friendly, for example, if you didn't have to press the ``k`` key for a ``k``, but - let's say - ``w``.

But now to the keyboards. All of them listed here have the correct alef. Nevertheless, many are problematic:

## Keyboards

### Platform independent keyboards

#### Hieroglyphic Keyboard from Keyman 

[Christian Casey](https://help.keyman.com/keyboard/hieroglyphic/1.4/hieroglyphic) has created a fantastic keyboard for writing Unicode hieroglyphics. However, there is no yod in the transcription, but an ``i``. Because of the missing yod you should use another keyboard for Egyptological transcription. But install it because of the Hieroglyphs!

### Keyboards for Mac

#### Mac Unicode Keyboards for the transliteration of Egyptian Hieroglyphs
For the Apple universe, [Serge Rosmorduc's](https://github.com/rosmord/mac_transliteration_keyboards) keyboard is the standard. It has correct alef, ayin and yod, it has capital letters. There are small limitations: we did not find a ʾ. Did we miss that, perhaps?

#### Unicode keyboard layout BBAW-BTS
Eliese-Sophia Lincke created this [keyboard](https://www.archaeologie.hu-berlin.de/de/aknoa/service/links/links) in 2020, but does not include the correct yod.

#### Unicode keyboard layouts (sic!) EGYDW-DE
Daniel Werning created this [keyboard](https://www.archaeologie.hu-berlin.de/de/aknoa/service/links/links) in 2018, so it does not contain the correct yod.

#### Conclusion
Please use the keyboard by Serge Rosmorduc!

### Keyboards for Windows

#### Unicode keyboard layout EGYDW-DE = Egyptological transcription - German
Daniel Werning created this [keyboard](https://www.archaeologie.hu-berlin.de/de/aknoa/service/links/links) in 2018, so it does not contain the correct yod. Furthermore, the keyboard is buggy, as it can crash Java programs.

#### Keyboard AAEW
Simon Schweitzer created this [keyboard](https://github.com/thesaurus-linguae-aegyptiae/keyboard-unicode-transliteration) in 2021, but it does not contain the correct yod.

#### MdC2Unicode keyboard
Daniel Werning created this [keyboard](https://github.com/thesaurus-linguae-aegyptiae/keyboard-mdc2unicode) in 2022. It is the only keyboard for Windows known to us that contains the correct yod. Thus it is the only keyboard that could be used on Windows. But it has some oddities that prevent us from recommending it without reservation:

* The capital letters are not created intuitively. For example, a ``SHIFT + k`` does not produce a ``K``, but a ``ḳ``.
* Characters like ø are missing.
* Besides the deprecated brackets 〈 and 〉, you can also produce ⟨ and ⟩ with this keyboard. However, these are by no means the recommended replacement for the deprecated brackets. ⟨ and ⟩ are reserved for mathematical and technical use. For other cases, use 〈 and 〉, see <https://en.wikipedia.org/w/index.php?title=Unicode_character_property&oldid=1114571327>.
* There is a •. This is the bullet. Perhaps this was intended to encode the verse point. Another punctuation mark would be more appropriate for this, such as the middle dot ·.

#### Conclusion

Dear developers who so diligently created keyboards, do not be angry with us, but this is - because of the lack of yod - our view: You can't really be happy with any keyboard on Windows. Only MdC2Unicode keyboard offers the right yod. But we can't really recommend this keyboard for the reasons mentioned above. Do we have to make our own keyboard with [Keyman Developer](https://keyman.com/developer/) or have we overlooked a suitable one? In any case, the keyboards can be made quickly. In this respect, this overview will hopefully become obsolete very soon.
