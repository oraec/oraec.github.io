# Four challenges when converting AES

After [Wikisource](https://github.com/oraec/formerly-mdc-now_unicode/tree/main/wikisource) and the [MdC texts from JSesh](https://github.com/oraec/formerly-mdc-now_unicode/tree/main/jsesh), we now take on the next resource to convert Egyptian texts to Unicode: [AES](https://github.com/simondschweitzer/aes)

This is a repo for corpus linguistic research. It contains more than 100000 Egyptian sentences from a total of 13026 texts. These sentences contain single words, so called tokens. The tokens have an Egyptological transcription, but not necessarily encoded hieroglyphs. On the contrary! Most of the texts have no encoded hieroglyphs. Only 2799 texts are useful for our purposes because they have hieroglyphic encodings.

The hieroglyphs are encoded in [Manuel de Codage](https://en.wikipedia.org/w/index.php?title=Manuel_de_Codage&oldid=1012543887). So you will say: no problem, let's go! O.k., but we have found four challenges, which we would like to present here in the blog.

## Text oriented vs. token oriented approach

The previous sources were text oriented. They are about creating a continuous text as a script from the Egyptian original. AES, on the other hand, is token-oriented. AES does not create a continuous text from hieroglyphs or from Egyptological transcription. Instead, all information is assigned to the tokens. Instead of a 𓅓𓉐𓏤, AES splits that into 𓅓 and 𓉐𓏤 because 𓅓 belongs to the preposition `m` and 𓉐𓏤 belongs to the word for 'house' `pr`. AES is interested in the spellings of the words, not in the representation of the text as a whole. This can be problematic because the order of the tokens need not correspond to the order in the hieroglyphic text. Gods may be placed before other words out of reverence, cf. [Peust, Carsten: Die honorative Transposition in der ägyptischen Schrift. In: LingAeg 15. 2007, p. 93-135](https://archiv.ub.uni-heidelberg.de/propylaeumdok/volltexte/2016/3221) So: there is no guarantee that the order of the hieroglyphs is correct!

## Partial destruction of tokens

Unfortunately, Egyptian texts are today often destroyed and many are preserved only in parts. As said, AES is interested in the spellings of words. What do you do if the word form is partially broken? AES is very consistent there and has two different fields for the hieroglyphs: 'hiero' and 'hieroinventar'. If the word form is not destroyed, the encoding is in the field `hiero`. In case of partial destruction, the field is not filled. The field `hieroinventar` contains the set of hieroglyphs used in this spelling. Still visible hieroglyphs in case of partial destruction can be stored here, even if the complete original spelling of the word form cannot be reconstructed. This is consistent and also very useful for the purposes of AES. But then we have many problems. We can say, these hieroglyphs are used in the word form, because they are in `hieroinventar`. But `hiero` is empty, so we can't convert anything. In this case we have to code a `[⯑]`.

## So many merely variants and missing characters

In the [last conversion](https://oraec.github.io/2022/10/10/missing-unicode-characters-and-further-mapping-problems.html), we had to add 157 pairs to our mapping. In AES, there are 1045 cases for which there is no equivalent in the mapping! This is a very large number that we cannot process in a hurry. We are considering how to engage the Egyptological community to assess these cases. Maybe we'll set up a wiki. For now, we will code a `�` in this 1045 cases because it is probably mostly just a variant of an existing character.

## Incomprehensible names of the texts

In the last two conversions, we were able to reuse the speaking names of the texts. When you read an [Stelae_of_Naukratis](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/wikisource/Stelae_of_Naukratis.md) or an [P. BM 10474-Teaching of Amenemope](https://github.com/oraec/formerly-mdc-now_unicode/blob/main/jsesh/P.%20BM%2010474-Teaching%20of%20Amenemope.md), you have some idea what kind of text we are talking about. AES, on the other hand, has very long IDs for the texts that no one can remember. Who could guess that `QUFWZTEPLRE4NHKCPAJXGSAOSQ` stands for Shipwrecked Sailor or `V6ZARX53EFDGLL36WL3HB4ESQM` for Tale of Woe? Even worse, no one can remember these monstrosities. Why should we convert if then the texts have these horrible names? This is pointless. Instead, we are working on a system with stable text IDs that are easier to remember. Stay tuned!
