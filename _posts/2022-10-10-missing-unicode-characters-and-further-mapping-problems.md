# Missing Unicode characters and further mapping problems

Well, are you already waiting impatiently for our next blog? We wanted to convert more texts encoded in Manuel de Codage to Unicode, so we took Serge Rosmorduc's great [repo](https://github.com/rosmord/MDC-texts) and looked at the freely licensed texts. There are 112 of them.

O.k., what took so long? There is already a [mapping](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/complete_mapping.csv). Well, that was not enough. It had 1807 pairs so far. By working with these texts, 157 have been added. That's an increase of almost 9%!

But [we did it and converted the texts](https://github.com/oraec/formerly-mdc-now_unicode/tree/main/jsesh). In this blog we report on the difficulties of the process.

First, we found twelve characters for which there are no corresponding Unicode characters. That is, first, no character had the required feature set, and second, the character could not be understood as a glyph of an existing character.

## Missing Unicode characters

### A158

![A158](https://hieroglyphes.pagesperso-orange.fr/A/A158.gif)

- phonetic value: nḥp
- source: Leitz, Christian: Quellentexte zur Ägyptischen Religion I. Die Tempelinschriften der griechisch-römischen Zeit. 2004, p. 154.
- source: <https://thotsignlist.org/mysign?id=223>

### A457

![A457](https://hieroglyphes.pagesperso-orange.fr/A/A457.gif)

- semantic value: Iunmutef priest
- source: Urk. IV, 157.11
- source: Rummel, Ute: Pfeiler seiner Mutter - Beistand seines Vaters : Untersuchungen zum Gott Iunmutef vom Alten Reich bis zum Ende des Neuen Reiches. Volume I. 2003. <https://nbn-resolving.org/urn%3Anbn%3Ade%3Agbv%3A18-34441>, p. 4 with n. 34.

### B24

![B24](https://hieroglyphes.pagesperso-orange.fr/B/B24.gif)

- semantic value: woman-shaped statue
- source: Polis, Stéphane & Rosmorduc, Serge. The Hieroglyphic Sign Functions. Suggestions for a Revised Taxonomy. In: Fuzzy Boundaries: Festschrift für Antonio Loprieno. 2015, p. 161.
- source: <http://tla-temp.hieroglyphic-texts.net/Belege_fuer_Hieroglyphe_B24_satzweise_Ansicht_.html>

### C165

![C165](https://hieroglyphes.pagesperso-orange.fr/C/C165.gif)

- semantic value: Mehit
- source: Leitz, Christian: Quellentexte zur Ägyptischen Religion I. Die Tempelinschriften der griechisch-römischen Zeit. 2004, p. 157.

### D153

![D153](https://hieroglyphes.pagesperso-orange.fr/D/D153.gif)

- phonetic value: r
- source: Leitz, Christian: Quellentexte zur Ägyptischen Religion I. Die Tempelinschriften der griechisch-römischen Zeit. 2004, p. 157.
- source: <https://thotsignlist.org/mysign?id=1943>

### F132

![F132](https://hieroglyphes.pagesperso-orange.fr/F/F132.gif)

- phonetic value: mꜣṯ
- source: Leitz, Christian: Quellentexte zur Ägyptischen Religion I. Die Tempelinschriften der griechisch-römischen Zeit. 2004, p. 162.

### M163

![M163](https://hieroglyphes.pagesperso-orange.fr/M/M163.gif)

- phonetic value: sm
- source: De Meulenaere, Herman. Un titre memphite méconnu. In: Mélanges Mariette. BdE 32. 1961, p. 285-290.

### R88

![R88](https://hieroglyphes.pagesperso-orange.fr/R/R88.gif)

- phonetic value: mks
- source: Leitz, Christian: Quellentexte zur Ägyptischen Religion I. Die Tempelinschriften der griechisch-römischen Zeit. 2004, p. 170.

### S116

![S116](https://hieroglyphes.pagesperso-orange.fr/S/S116.gif)

- measure of linen, ligature of S114 4 times -> S114 is the representation of the missing Unicode character 
- source: Scheele, Katrin: Die Stofflisten des Alten Reiches. Lexikographie, Entwicklung und Gebrauch. MENES 2. 2005, p. 56-58.
- meaning not listed in https://thotsignlist.org/mysign?id=5651

### T92

![T92](https://hieroglyphes.pagesperso-orange.fr/T/T92.gif)

- semantic value: net/trap
- source: <https://thotsignlist.org/mysign?id=6023> (T90)

### U105

![U105](https://hieroglyphes.pagesperso-orange.fr/U/U105.gif)

- semantic value: saw
- source: <http://tla-temp.hieroglyphic-texts.net/Belege_fuer_Hieroglyphe_U105_satzweise_Ansicht_.html>

### <S

- opening of the serekh, cf. opening of ḥwt enclosure 𓉘; opening of fortified wall cartouche 𓊆; opening of square fortified wall cartouche 𓊈; opening of cartouche 𓍹

A ⯑ was used as a placeholder for the mapping. Hopefully, these characters will be added in the future.

## Glyphs instead of characters and other problems

However, most of the new 157 cases are variants of existing characters: An `N104` is just a variant of 𓈞, or a `D3A` is just a variant of 𓁸.

Remember the saying of Mark-Jan Nederhof we already had in a previous blog? No? We quote:

> In Egyptology however, there seem to be tendencies to remain true to the original manuscript while encoding a text, often to the extent of encoding glyphs rather than characters. (Nederhof, Mark-Jan. The Manuel de Codage encoding of hieroglyphs impedes development of corpora. In: Texts, Languages & Information Technology in Egyptology. Edited by Jean Winand & Stéphane Polis. 2013. 104.)

This statement is confirmed by the many addressed variants we found in the texts. Often the code of Manuel de Codage does not want to be a code at all, but merely represents the glyphs as similar as possible. Here is an impressive example: `R13{{282,0,92}}**D263{{126,240,51}}**D234{{49,599,58}}**W10{{0,670,41}}-W10:mw-!!!
R15{{442,0,92}}**D263{{126,91,51}}**D234{{49,450,58}}**W10{{0,521,41}}-W10:mw-!!`

This [code snippet](https://github.com/rosmord/MDC-texts/blob/7d3650124f582740335444f1cfdbff918b30af62/texts/Stela%20Louvre%20C%2026.gly#L17-L18) is from the [text](https://github.com/rosmord/MDC-texts/blob/master/texts/Stela%20Louvre%20C%2026.gly) for the [Stele Louvre C 26](https://collections.louvre.fr/en/ark:/53355/cl010025023). This represents the icons to the left and right of the udjat eyes. But the code suggests that `D263` and `D234` are used as characters there. But this is not true at all! `D263` and `D234` are there only because the character shapes help to reproduce the icon as a picture.

Another example: Occasionally there is a `1*1*1` in the code, but it is usually not the number 1, but the plural determinative 𓏥. Therefore, be careful when reusing our converted data. We cannot guarantee the quality of the data.

If the Egyptologists encode mainly glyphs, don't be surprised if some characters are chosen only for their similarity. As a result, one character suddenly has the most different functions. `Z30` shows impressively a big confusion in the coding practice. With such characters we had to map with `�`.

Undocumented code like `US85Aa1001XT` was also mapped with `�`.

Finally, there is also code that does not stand for a character at all. Space fillers have their own code in [JSesh](https://jsesh.qenherkhopeshef.org/glyphs/collection/61), but are not to be converted to Unicode.
