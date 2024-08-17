# Digitization of Coptic Etymologies

Dear all! A sign of life from us again after a long time! We have been busy with a big project, which we have now completed and would like to present to you in this blog.

The Egyptian language has the longest documented history in the world. About 5000 years of language history can be found in written documents. Of course, the Egyptian of the 4th millennium BC is not identical to the Egyptian of the Middle Ages. For this reason, Egyptian is divided into different language stages, which formed independent scientific traditions. The last language stage is called Coptic and is studied in the independent discipline of Coptology. Coptology has also developed an independent dictionary for Coptic, which is outstanding: [Crum, Coptic Dictionary](https://coptot.manuscriptroom.com/crum-coptic-dictionary) If you browse through it, you will notice that there are no references to the earlier language levels of Egyptian. So you wouldn't be able to tell whether a word listed by Crum was used in earlier times or not. Based on Crum, the ingenious digital service [Coptic Dictionary Online](https://coptic-dictionary.org/), the CDO, was created. This is the first place to go when looking for Coptic words and their translations. Not without reason, the Coptic Dictionary Online received a DH award. There is even access to a digital corpus of Coptic texts that can be searched in detail. Wow! But what is missing is the link to the earlier stages of the language. You don't learn that the preposition ⲉ goes back to the preposition r.

Where can I find this information? Coptology has three excellent reference works that list the internal Egyptian etymologies: [Cerny, Coptic Etymological Dictionary](https://aegyptiaca.uni-muenster.de/Record/51209), [Vycichl, Dictionnaire étymologique de la langue copte](https://aegyptiaca.uni-muenster.de/Record/46163), [Westendorf, Koptisches Handwörterbuch](https://aegyptiaca.uni-muenster.de/Record/104465) but these are all printed dictionaries with no digital representation. This is where our project comes in. We analyzed these sources and created links between the digital entries. The starting point was the Coptic word list that forms the basis of the [CDO](https://coptic-dictionary.org/). The data is available as XML in a [Github repository](https://github.com/KELLIA/dictionary). If the Coptic word has a predecessor in Demotic (Demotic is the penultimate language stage of Egyptian, directly preceding Coptic), we noted the ID of the Demotic word in the [TLA](https://aaew.bbaw.de/tla). We found 1827 relationships between Coptic and Demotic words. However, we suspect that there are many more Demotic antecedents of Coptic words. This is because recent Demotic studies have uncovered many new texts that were not known to the above-mentioned etymological dictionaries, all of which date from the 20th century. If you know of a new etymology that we have not listed, please send us an e-mail! Of course, we also searched for antecedents preserved in hieroglyphic or hieratic texts. In these cases, we compared the antecedents with the lexical entries in our [ORAEC corpus](https://oraec.github.io/corpus). In this way, we created a link between the Coptic word from the CDO and the Egyptian word from ORAEC. This resulted in 1695 relations. In total, we determined the pre-Coptic antecedents of 2177 Coptic words. The results show that for a number of Coptic words both an Egyptian and a Demotic antecedent are known.

The relations are published as csv in a [Github repository](https://github.com/oraec/coptic_etymologies). See the readme for more details. The most important thing is that we have released our work under the freest license, cc 0, so that anyone can use and process the data as they wish. Such a CSV is not very user friendly because it only lists IDs. That's why I put a list of Coptic words with Egyptian etymology here on the blog. The first column lists the Coptic words associated with the CDO. The second column lists the Egyptian words. The link there leads to the overview pages of the word in ORAEC, so that you can quickly get an overview of the references. The third column contains the Demotic words linked to the TLA.

| Coptic | Egyptian | Demotic |
| ------ | -------- | ------- |
| [ⲁ-](https://coptic-dictionary.org/entry.cgi?tla=C5) (ID:C5) | [ꜥ.t](https://oraec.github.io/corpus/854495.html) |  |
| [ⲁⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6) (ID:C6) | [ꜥbꜣ.yt](https://oraec.github.io/corpus/36610.html) |  |
| [ⲁⲃⲱⲕ](https://coptic-dictionary.org/entry.cgi?tla=C9) (ID:C9) |  | [ꜥbq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=928&db=1) |
| [ⲁⲃⲥⲱⲛ](https://coptic-dictionary.org/entry.cgi?tla=C14) (ID:C14) | [jbzꜣ](https://oraec.github.io/corpus/23930.html) |  |
| [ⲁⲃⲏϣ](https://coptic-dictionary.org/entry.cgi?tla=C15) (ID:C15) | [ꜣbḫ.t](https://oraec.github.io/corpus/92.html) |  |
| [ⲁⲓⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C18) (ID:C18) | [ꜥb.w](https://oraec.github.io/corpus/36300.html) |  |
| [ⲁⲉⲓⲕ](https://coptic-dictionary.org/entry.cgi?tla=C24) (ID:C24) | [ꜥq.y](https://oraec.github.io/corpus/41430.html) | [ꜥyq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=875&db=1) |
| [ⲁⲕⲱ](https://coptic-dictionary.org/entry.cgi?tla=C29) (ID:C29) | [ꜣq.yt](https://oraec.github.io/corpus/294.html) |  |
| [ⲁⲕⲱⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C32) (ID:C32) | [jkn](https://oraec.github.io/corpus/32610.html) |  |
| [ⲁⲕⲏⲥ](https://coptic-dictionary.org/entry.cgi?tla=C33) (ID:C33) | [ꜥgsw](https://oraec.github.io/corpus/41800.html) |  |
| [ⲁⲗ](https://coptic-dictionary.org/entry.cgi?tla=C35) (ID:C35) |  | [ꜥlwꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1060&db=1) |
| [ⲁⲗ](https://coptic-dictionary.org/entry.cgi?tla=C36) (ID:C36) | [ꜥr](https://oraec.github.io/corpus/39180.html) | [ꜥl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1052&db=1) |
| [ⲁⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C37) (ID:C37) | [jꜥr](https://oraec.github.io/corpus/21770.html) | [ꜥl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1051&db=1) |
| [ⲁⲗⲓ](https://coptic-dictionary.org/entry.cgi?tla=C46) (ID:C46) | [jꜣr.w](https://oraec.github.io/corpus/20810.html) |  |
| [ⲁⲗⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C49) (ID:C49) |  | [ꜥlw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1059&db=1) |
| [ⲁⲗⲱ](https://coptic-dictionary.org/entry.cgi?tla=C53) (ID:C53) | [wꜣr.t](https://oraec.github.io/corpus/42980.html) |  |
| [ⲁⲗⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C54) (ID:C54) | [ꜥrq.y](https://oraec.github.io/corpus/39740.html) | [ꜥrqy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1045&db=1) |
| [ⲁⲗⲓⲗ](https://coptic-dictionary.org/entry.cgi?tla=C61) (ID:C61) |  | [ꜥlꜥl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1057&db=1) |
| [ⲁⲗⲱⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C64) (ID:C64) | [ꜥr](https://oraec.github.io/corpus/39180.html) | [ꜥl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1052&db=1) |
| [ⲁⲗⲱⲟⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C74) (ID:C74) | [ꜥr.t](https://oraec.github.io/corpus/39210.html) | [ꜥrwe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1427&db=1) |
| [ⲁⲗⲟϭ](https://coptic-dictionary.org/entry.cgi?tla=C78) (ID:C78) | [ꜥrq](https://oraec.github.io/corpus/39610.html) | [ꜥkl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1142&db=1) |
| [ⲁⲗⲟϭ](https://coptic-dictionary.org/entry.cgi?tla=C79) (ID:C79) | [ꜥrq](https://oraec.github.io/corpus/39610.html) | [ꜥkl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1142&db=1) |
| [ⲁⲁⲙ](https://coptic-dictionary.org/entry.cgi?tla=C80) (ID:C80) | [ꜥꜥꜣm](https://oraec.github.io/corpus/35700.html) |  |
| [ⲁⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C82) (ID:C82) | [ꜥꜣm](https://oraec.github.io/corpus/35400.html) | [ꜥꜣm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=854&db=1) |
| [ⲁⲙⲁⲗⲏϫ](https://coptic-dictionary.org/entry.cgi?tla=C86) (ID:C86) | [knm](https://oraec.github.io/corpus/164780.html) |  |
| [ⲁⲙⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C89) (ID:C89) | [mn](https://oraec.github.io/corpus/69630.html) | [mn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2424&db=1) |
| [ⲁⲙⲟⲩⲛ](https://coptic-dictionary.org/entry.cgi?tla=C100) (ID:C100) | [Jmn](https://oraec.github.io/corpus/26060.html) | [Jmn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=505&db=1) |
| [ⲁⲙⲓⲛⲁⲕⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C101) (ID:C101) |  | [ꜣmwnyꜥk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=107&db=1) |
| [ⲁⲙⲛⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C102) (ID:C102) | [jmn.tjt](https://oraec.github.io/corpus/26180.html) | [jmnt.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-127&db=1) |
| [ⲁⲙⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C103) (ID:C103) |  | [ꜥmr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=970&db=1) |
| [ⲁⲙⲣⲏϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C106) (ID:C106) | [mrḥ](https://oraec.github.io/corpus/72800.html) | [mrḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2552&db=1) |
| [ⲁⲙϣⲓ](https://coptic-dictionary.org/entry.cgi?tla=C108) (ID:C108) | [mḫꜣ](https://oraec.github.io/corpus/74240.html) |  |
| [ⲁⲙϩⲣⲏⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C109) (ID:C109) |  | [mẖrr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2665&db=1) |
| [ⲁⲙⲁϩⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C110) (ID:C110) |  | [ꜣmḥṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=111&db=1) |
| [ⲁⲛ](https://coptic-dictionary.org/entry.cgi?tla=C120) (ID:C120) | [jn](https://oraec.github.io/corpus/26700.html) | [jn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=529&db=1) |
| [ⲁⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C121) (ID:C121) | [ꜥꜣ](https://oraec.github.io/corpus/34760.html) |  |
| [ⲁⲛⲍⲏⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C125) (ID:C125) | [ꜥ.t-sbꜣ.w](https://oraec.github.io/corpus/34730.html) | [ꜥ.t-n-sbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=799&db=1) |
| [ⲁⲛⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C126) (ID:C126) | [ꜥni̯](https://oraec.github.io/corpus/38070.html) |  |
| [ⲁⲛⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C127) (ID:C127) | [ꜥn.w](https://oraec.github.io/corpus/600622.html) | [ꜥn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7797&db=1) |
| [ⲁⲛⲑⲟⲩⲥ](https://coptic-dictionary.org/entry.cgi?tla=C133) (ID:C133) | [ḥntꜣsw](https://oraec.github.io/corpus/107380.html) | [ḥnṱs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1410&db=1) |
| [ⲁⲛⲟⲕ](https://coptic-dictionary.org/entry.cgi?tla=C135) (ID:C135) | [jnk](https://oraec.github.io/corpus/27940.html) | [jnky](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=590&db=1) |
| [ⲁⲛⲓⲕⲁⲙ](https://coptic-dictionary.org/entry.cgi?tla=C137) (ID:C137) | [jnr-km](https://oraec.github.io/corpus/27660.html) | [jny-km](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3080&db=1) |
| [ⲁⲛⲟⲙ](https://coptic-dictionary.org/entry.cgi?tla=C138) (ID:C138) | [jnm](https://oraec.github.io/corpus/27420.html) | [ꜣnmm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=124&db=1) |
| [ⲁⲛⲟⲛ](https://coptic-dictionary.org/entry.cgi?tla=C142) (ID:C142) | [jnn](https://oraec.github.io/corpus/27490.html) | [jnn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=582&db=1) |
| [ⲁⲛⲟⲩⲡ](https://coptic-dictionary.org/entry.cgi?tla=C145) (ID:C145) | [Jnp.w](https://oraec.github.io/corpus/27360.html) | [Jnp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=579&db=1) |
| [ⲁⲛⲁϣ](https://coptic-dictionary.org/entry.cgi?tla=C154) (ID:C154) | [ꜥnḫ](https://oraec.github.io/corpus/38560.html) | [ꜥnḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=996&db=1) |
| [ⲁⲛⲁϣ](https://coptic-dictionary.org/entry.cgi?tla=C158) (ID:C158) | [ꜥnḫ](https://oraec.github.io/corpus/38590.html) | [ꜥnḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=998&db=1) |
| [ⲁⲛϣⲓⲣⲓ](https://coptic-dictionary.org/entry.cgi?tla=C159) (ID:C159) |  | [ꜣnḏrꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=133&db=1) |
| [ⲁⲛϩ](https://coptic-dictionary.org/entry.cgi?tla=C161) (ID:C161) | [jnḥ.w](https://oraec.github.io/corpus/27730.html) | [jnḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-43&db=1) |
| [ⲁⲛϩⲟⲩⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C163) (ID:C163) | [Jn-ḥr.t](https://oraec.github.io/corpus/26850.html) | [Jn-ḥr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=566&db=1) |
| [ⲁⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C165) (ID:C165) | [tp.t](https://oraec.github.io/corpus/170920.html) | [ꜥpe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=930&db=1) |
| [ⲁⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C11276) (ID:C11276) | [tp.t](https://oraec.github.io/corpus/170920.html) | [ꜥpe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=930&db=1) |
| [ⲁⲡⲉⲓ](https://coptic-dictionary.org/entry.cgi?tla=C174) (ID:C174) | [jpꜣ](https://oraec.github.io/corpus/24250.html) |  |
| [ⲁⲡⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C179) (ID:C179) |  | [jpt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=473&db=1) |
| [ⲁⲣⲁ](https://coptic-dictionary.org/entry.cgi?tla=C182) (ID:C182) | [jr.j-ꜥꜣ](https://oraec.github.io/corpus/28730.html) | [jry-ꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-38&db=1) |
| [ⲁⲣⲁ](https://coptic-dictionary.org/entry.cgi?tla=C183) (ID:C183) | [jr.j-ꜥꜣ](https://oraec.github.io/corpus/28730.html) | [jry-ꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-38&db=1) |
| [ⲁⲣⲏⲃ](https://coptic-dictionary.org/entry.cgi?tla=C188) (ID:C188) |  | [ꜣlb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=174&db=1) |
| [ⲁⲣⲏⲩ](https://coptic-dictionary.org/entry.cgi?tla=C197) (ID:C197) |  | [ꜥrw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1033&db=1) |
| [ⲁⲣⲟϣ](https://coptic-dictionary.org/entry.cgi?tla=C200) (ID:C200) |  | [jrš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=650&db=1) |
| [ⲁⲣϣⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C202) (ID:C202) | [ꜥršn](https://oraec.github.io/corpus/39590.html) | [ꜥršyn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7537&db=1) |
| [ⲁⲣⲏϫ⸗](https://coptic-dictionary.org/entry.cgi?tla=C204) (ID:C204) | [ḏr.w](https://oraec.github.io/corpus/184990.html) |  |
| [ⲁⲥ](https://coptic-dictionary.org/entry.cgi?tla=C207) (ID:C207) | [jz](https://oraec.github.io/corpus/31040.html) | [jsy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=692&db=1) |
| [ⲁⲥⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C213) (ID:C213) | [jsw](https://oraec.github.io/corpus/31330.html) | [jswy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=703&db=1) |
| [ⲁⲥⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C216) (ID:C216) | [jzj](https://oraec.github.io/corpus/31240.html) | [ꜣsw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-650&db=1) |
| [ⲁⲥⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C225) (ID:C225) |  | [ꜣspy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=220&db=1) |
| [ⲁⲥⲏⲣ](https://coptic-dictionary.org/entry.cgi?tla=C226) (ID:C226) | [wsr.w](https://oraec.github.io/corpus/49600.html) | [wsr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-8037&db=1) |
| [ⲁⲥⲟⲩⲓ](https://coptic-dictionary.org/entry.cgi?tla=C227) (ID:C227) | [jns](https://oraec.github.io/corpus/27860.html) | [ꜣswꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=218&db=1) |
| [ⲁⲧ-](https://coptic-dictionary.org/entry.cgi?tla=C233) (ID:C233) | [jw.tj](https://oraec.github.io/corpus/22030.html) | [jwty](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=432&db=1) |
| [ⲁⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C235) (ID:C235) | [jꜣd.t](https://oraec.github.io/corpus/21190.html) | [ꜣte.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=259&db=1) |
| [ⲁⲧⲟⲩⲙ](https://coptic-dictionary.org/entry.cgi?tla=C237) (ID:C237) | [Jtm.w](https://oraec.github.io/corpus/33040.html) | [Jtm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=735&db=1) |
| [ⲁⲩⲁⲛ](https://coptic-dictionary.org/entry.cgi?tla=C241) (ID:C241) | [jwn](https://oraec.github.io/corpus/22570.html) | [jwn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=404&db=1) |
| [ⲁⲩⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C245) (ID:C245) | [jn.wt](https://oraec.github.io/corpus/27090.html) | [jwn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=403&db=1) |
| [ⲁⲩⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C247) (ID:C247) | [jwd.t](https://oraec.github.io/corpus/23240.html) |  |
| [ⲁⲫⲱⲫ](https://coptic-dictionary.org/entry.cgi?tla=C249) (ID:C249) | [Ꜥꜣpp](https://oraec.github.io/corpus/35360.html) | [ꜥpp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-759&db=1) |
| [ⲁϣ](https://coptic-dictionary.org/entry.cgi?tla=C250) (ID:C250) | [jḫ](https://oraec.github.io/corpus/30740.html) | [jḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=673&db=1) |
| [ⲁϣ](https://coptic-dictionary.org/entry.cgi?tla=C251) (ID:C251) | [jḫ](https://oraec.github.io/corpus/30740.html) | [jḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=673&db=1) |
| [ⲁϣ](https://coptic-dictionary.org/entry.cgi?tla=C252) (ID:C252) | [ꜥḫ](https://oraec.github.io/corpus/40500.html) | [ꜥḫe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1083&db=1) |
| [ⲁϣⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C255) (ID:C255) | [ꜥšꜣ](https://oraec.github.io/corpus/41010.html) | [ꜥšꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1112&db=1) |
| [ⲟϣ](https://coptic-dictionary.org/entry.cgi?tla=C256) (ID:C256) | [ꜥšꜣ](https://oraec.github.io/corpus/41010.html) | [ꜥšꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1112&db=1) |
| [ⲁϣⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C257) (ID:C257) | [ꜥšꜣ](https://oraec.github.io/corpus/41020.html) | [ꜥšꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-6425&db=1) |
| [ⲁϣⲏ](https://coptic-dictionary.org/entry.cgi?tla=C261) (ID:C261) | [ꜥšꜣ.wt](https://oraec.github.io/corpus/41050.html) | [ꜥšꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1113&db=1) |
| [ⲁϣⲓⲣⲁ](https://coptic-dictionary.org/entry.cgi?tla=C262) (ID:C262) | [ꜥšꜣ](https://oraec.github.io/corpus/41040.html) |  |
| [ⲁϥ](https://coptic-dictionary.org/entry.cgi?tla=C266) (ID:C266) | [jwf](https://oraec.github.io/corpus/22520.html) | [jwf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=400&db=1) |
| [ⲁϥ](https://coptic-dictionary.org/entry.cgi?tla=C270) (ID:C270) | [ꜥff](https://oraec.github.io/corpus/37370.html) | [ꜥf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=941&db=1) |
| [ⲁϥ](https://coptic-dictionary.org/entry.cgi?tla=C271) (ID:C271) | [ꜥff](https://oraec.github.io/corpus/37370.html) | [ꜥf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=941&db=1) |
| [ⲁϥϫⲓⲣ](https://coptic-dictionary.org/entry.cgi?tla=C275) (ID:C275) | [ꜣfi̯](https://oraec.github.io/corpus/119.html) | [ꜣfꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=99&db=1) |
| [ⲁϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C284) (ID:C284) | [ꜥḥꜥ.w](https://oraec.github.io/corpus/40480.html) | [ꜥḥꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1073&db=1) |
| [ⲁϩⲟ](https://coptic-dictionary.org/entry.cgi?tla=C291) (ID:C291) | [ꜥḥꜥ.w](https://oraec.github.io/corpus/40280.html) |  |
| [ⲁϩⲟⲙ](https://coptic-dictionary.org/entry.cgi?tla=C295) (ID:C295) | [jhm](https://oraec.github.io/corpus/850149.html) | [ꜣhm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=189&db=1) |
| [ⲁϩⲱⲙ](https://coptic-dictionary.org/entry.cgi?tla=C296) (ID:C296) | [ꜥẖm](https://oraec.github.io/corpus/858543.html) | [ꜥẖm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1095&db=1) |
| [ⲁϩⲁⲛ](https://coptic-dictionary.org/entry.cgi?tla=C297) (ID:C297) | [r-hn-r](https://oraec.github.io/corpus/98590.html) | [r-hn-r](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3378&db=1) |
| [ⲁϩⲣ](https://coptic-dictionary.org/entry.cgi?tla=C298) (ID:C298) |  | [ꜣẖy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=204&db=1) |
| [ⲁϩⲣⲟ⸗](https://coptic-dictionary.org/entry.cgi?tla=C299) (ID:C299) |  | [jḫ-r=](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-400&db=1) |
| [ⲁϫⲱ](https://coptic-dictionary.org/entry.cgi?tla=C301) (ID:C301) | [Wꜣḏ.t](https://oraec.github.io/corpus/43760.html) | [Wꜣḏ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1227&db=1) |
| [ⲁϭⲃⲉⲥ](https://coptic-dictionary.org/entry.cgi?tla=C303) (ID:C303) | [ꜣgb.w](https://oraec.github.io/corpus/314.html) |  |
| [ⲁϭⲟⲗⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C304) (ID:C304) |  | [ꜥklṱꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1143&db=1) |
| [ⲁϭⲛⲓ](https://coptic-dictionary.org/entry.cgi?tla=C305) (ID:C305) | [ꜥḏn.t](https://oraec.github.io/corpus/863009.html) | [ꜥḏn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1166&db=1) |
| [ⲁϭⲛⲓ](https://coptic-dictionary.org/entry.cgi?tla=C306) (ID:C306) | [ꜥḏn.t](https://oraec.github.io/corpus/863009.html) | [ꜥḏn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1166&db=1) |
| [ⲁϭⲟⲛ](https://coptic-dictionary.org/entry.cgi?tla=C312) (ID:C312) | [ꜥgn](https://oraec.github.io/corpus/41730.html) | [ꜥkn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1137&db=1) |
| [ⲃⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C318) (ID:C318) | [bꜥj](https://oraec.github.io/corpus/54870.html) | [bꜥy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1677&db=1) |
| [ⲃⲁ](https://coptic-dictionary.org/entry.cgi?tla=C319) (ID:C319) | [bꜥj](https://oraec.github.io/corpus/54870.html) | [bꜥy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1677&db=1) |
| [ⲃⲏ](https://coptic-dictionary.org/entry.cgi?tla=C322) (ID:C322) | [bꜣ.y](https://oraec.github.io/corpus/53190.html) | [bꜥy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1678&db=1) |
| [ⲃⲱ](https://coptic-dictionary.org/entry.cgi?tla=C323) (ID:C323) | [bꜣ.t](https://oraec.github.io/corpus/52960.html) | [be](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1619&db=1) |
| [ⲃⲁⲁⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C324) (ID:C324) | [ꜥbꜥb](https://oraec.github.io/corpus/36660.html) |  |
| [ⲃⲉⲉⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C329) (ID:C329) | [bꜥbꜥ](https://oraec.github.io/corpus/54900.html) |  |
| [ⲃⲏⲃ](https://coptic-dictionary.org/entry.cgi?tla=C333) (ID:C333) | [bꜣbꜣ](https://oraec.github.io/corpus/53420.html) |  |
| [ⲃⲟⲩⲃⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C336) (ID:C336) | [ꜥbꜥb](https://oraec.github.io/corpus/36670.html) | [bwbwe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1700&db=1) |
| [ⲃⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C338) (ID:C338) |  | [by](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1648&db=1) |
| [ⲃⲟⲓⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C341) (ID:C341) | [bjn.t](https://oraec.github.io/corpus/54650.html) | [byn.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1660&db=1) |
| [ⲃⲉⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C350) (ID:C350) | [bꜣk.w](https://oraec.github.io/corpus/53820.html) | [bꜣk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1809&db=1) |
| [ⲃⲏⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C361) (ID:C361) | [bꜣk](https://oraec.github.io/corpus/53840.html) | [bꜣk.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-236&db=1) |
| [ⲃⲟⲕⲓ](https://coptic-dictionary.org/entry.cgi?tla=C363) (ID:C363) | [bkꜣ](https://oraec.github.io/corpus/57820.html) | [bk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-6256&db=1) |
| [ⲃⲱⲕ](https://coptic-dictionary.org/entry.cgi?tla=C391) (ID:C391) | [bꜣk](https://oraec.github.io/corpus/53830.html) | [bꜣk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1810&db=1) |
| [ⲃⲱⲕⲓ](https://coptic-dictionary.org/entry.cgi?tla=C397) (ID:C397) | [bꜣk.t](https://oraec.github.io/corpus/53870.html) | [bꜣk.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1818&db=1) |
| [ⲃⲁⲗ](https://coptic-dictionary.org/entry.cgi?tla=C400) (ID:C400) | [br](https://oraec.github.io/corpus/56270.html) | [bl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1756&db=1) |
| [ⲃⲱⲗ](https://coptic-dictionary.org/entry.cgi?tla=C404) (ID:C404) | [bnu̯](https://oraec.github.io/corpus/55510.html) | [blꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1759&db=1) |
| [ⲃⲟⲗ](https://coptic-dictionary.org/entry.cgi?tla=C415) (ID:C415) | [bnr.w](https://oraec.github.io/corpus/55920.html) | [bnr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1735&db=1) |
| [ⲉⲃⲟⲗ](https://coptic-dictionary.org/entry.cgi?tla=C417) (ID:C417) | [r-bnr](https://oraec.github.io/corpus/91970.html) | [r-bnr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3369&db=1) |
| [ⲛⲃⲟⲗ](https://coptic-dictionary.org/entry.cgi?tla=C420) (ID:C420) |  | [n-bnr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2919&db=1) |
| [ⲛⲃⲗ-](https://coptic-dictionary.org/entry.cgi?tla=C421) (ID:C421) | [n-bnr](https://oraec.github.io/corpus/79140.html) | [n-bnr=](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1389&db=1) |
| [ⲣⲃⲟⲗ](https://coptic-dictionary.org/entry.cgi?tla=C435) (ID:C435) |  | [jr-bnr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-75&db=1) |
| [ⲃⲟⲗⲃⲗ](https://coptic-dictionary.org/entry.cgi?tla=C439) (ID:C439) |  | [blbl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1767&db=1) |
| [ⲃⲗⲃⲓⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C442) (ID:C442) | [bnn.t](https://oraec.github.io/corpus/55890.html) | [blbylꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1765&db=1) |
| [ⲃⲗⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C449) (ID:C449) |  | [bl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1757&db=1) |
| [ⲃⲁⲗⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C454) (ID:C454) | [bnd](https://oraec.github.io/corpus/56240.html) |  |
| [ⲃⲓⲗⲧⲓ](https://coptic-dictionary.org/entry.cgi?tla=C455) (ID:C455) | [mn.t](https://oraec.github.io/corpus/69800.html) | [mne.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2440&db=1) |
| [ⲃⲗϩⲙⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C456) (ID:C456) |  | [Blhmwt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1768&db=1) |
| [ⲃⲗϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C457) (ID:C457) | [bḏꜣ](https://oraec.github.io/corpus/58570.html) | [blḏ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3682&db=1) |
| [ⲃⲗϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C458) (ID:C458) | [bḏꜣ](https://oraec.github.io/corpus/58570.html) | [blḏ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3682&db=1) |
| [ⲃⲁⲁⲙⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C461) (ID:C461) | [bꜣ-n-p.t](https://oraec.github.io/corpus/53060.html) | [by-ꜥꜣ-n-p.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1653&db=1) |
| [ⲃⲁⲁⲙⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C462) (ID:C462) | [bꜣ-n-p.t](https://oraec.github.io/corpus/53060.html) | [by-ꜥꜣ-n-p.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1653&db=1) |
| [ⲃⲏⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C466) (ID:C466) | [mn.t](https://oraec.github.io/corpus/69780.html) | [bny.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1723&db=1) |
| [ⲃⲏⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C467) (ID:C467) | [mn.t](https://oraec.github.io/corpus/69780.html) | [bny.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1723&db=1) |
| [ⲃⲓⲛⲓ](https://coptic-dictionary.org/entry.cgi?tla=C469) (ID:C469) | [mn.t](https://oraec.github.io/corpus/69820.html) |  |
| [ⲃⲱⲱⲛ](https://coptic-dictionary.org/entry.cgi?tla=C470) (ID:C470) | [bjn](https://oraec.github.io/corpus/54605.html) | [byn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1646&db=1) |
| [ⲃⲟⲟⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C471) (ID:C471) | [bjn](https://oraec.github.io/corpus/54605.html) | [byn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1646&db=1) |
| [ⲃⲟⲟⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C472) (ID:C472) | [bjn.t](https://oraec.github.io/corpus/54640.html) | [byn.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-287&db=1) |
| [ⲃⲛⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C484) (ID:C484) | [bnj](https://oraec.github.io/corpus/55930.html) | [bne.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1708&db=1) |
| [ϣⲛⲃⲛⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C490) (ID:C490) |  | [šn-bne.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4522&db=1) |
| [ⲃⲉⲛⲓⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C491) (ID:C491) | [bjꜣ-n-p.t](https://oraec.github.io/corpus/54450.html) | [bnpy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1731&db=1) |
| [ⲃⲟⲛⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C492) (ID:C492) | [bnd.t](https://oraec.github.io/corpus/850454.html) | [bnṱy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-805&db=1) |
| [ⲃⲓⲛⲁϫ](https://coptic-dictionary.org/entry.cgi?tla=C496) (ID:C496) |  | [pynꜥks](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1946&db=1) |
| [ⲃⲓⲣ](https://coptic-dictionary.org/entry.cgi?tla=C499) (ID:C499) |  | [byr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1662&db=1) |
| [ⲃⲓⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C500) (ID:C500) |  | [byr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1662&db=1) |
| [ⲃⲁⲁⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C501) (ID:C501) | [bjr](https://oraec.github.io/corpus/56310.html) | [byry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1665&db=1) |
| [ⲃⲱⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C502) (ID:C502) | [br](https://oraec.github.io/corpus/56320.html) |  |
| [ⲃⲱⲱⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C503) (ID:C503) | [bnn](https://oraec.github.io/corpus/55820.html) |  |
| [ⲃⲉⲣⲃⲓⲣ](https://coptic-dictionary.org/entry.cgi?tla=C512) (ID:C512) | [bnbn](https://oraec.github.io/corpus/55720.html) | [bnbn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1729&db=1) |
| [ⲃⲣⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C516) (ID:C516) |  | [bry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1743&db=1) |
| [ⲃⲁⲣⲱϩ](https://coptic-dictionary.org/entry.cgi?tla=C534) (ID:C534) |  | [brḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1749&db=1) |
| [ⲃⲣϭⲟⲟⲩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C537) (ID:C537) | [mrkbt](https://oraec.github.io/corpus/73010.html) |  |
| [ⲃⲁⲥ](https://coptic-dictionary.org/entry.cgi?tla=C538) (ID:C538) | [bꜣs](https://oraec.github.io/corpus/53600.html) | [bs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1787&db=1) |
| [ⲃⲏⲥ](https://coptic-dictionary.org/entry.cgi?tla=C540) (ID:C540) | [Bs](https://oraec.github.io/corpus/57210.html) | [Bs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1786&db=1) |
| [ⲃⲉⲥⲛⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C542) (ID:C542) |  | [bsnṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1795&db=1) |
| [ⲃⲏⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C553) (ID:C553) | [bꜣd.t](https://oraec.github.io/corpus/54070.html) |  |
| [ⲃⲟⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C555) (ID:C555) | [btꜣ.w](https://oraec.github.io/corpus/58130.html) | [bty.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1834&db=1) |
| [ⲃⲟⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C556) (ID:C556) | [btꜣ.w](https://oraec.github.io/corpus/58130.html) | [btwe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1836&db=1) |
| [ⲃⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C562) (ID:C562) | [btꜣ](https://oraec.github.io/corpus/58140.html) | [bty](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1833&db=1) |
| [ⲃⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C563) (ID:C563) | [bd.t](https://oraec.github.io/corpus/58430.html) | [bd.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1831&db=1) |
| [ⲃⲱⲧⲥ (ⲉⲃⲟⲗ)](https://coptic-dictionary.org/entry.cgi?tla=C564) (ID:C564) | [bgs](https://oraec.github.io/corpus/450143.html) | [bgs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1828&db=1) |
| [ⲃⲱⲧⲥ](https://coptic-dictionary.org/entry.cgi?tla=C567) (ID:C567) | [bgs.w](https://oraec.github.io/corpus/58060.html) | [bgs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1828&db=1) |
| [ⲃⲁⲧⲥ](https://coptic-dictionary.org/entry.cgi?tla=C572) (ID:C572) | [bgs.w](https://oraec.github.io/corpus/58060.html) | [bgs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1828&db=1) |
| [ⲃⲏⲩ](https://coptic-dictionary.org/entry.cgi?tla=C575) (ID:C575) | [bw.t](https://oraec.github.io/corpus/55150.html) | [bw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1691&db=1) |
| [ⲃⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C576) (ID:C576) | [bꜣw](https://oraec.github.io/corpus/850444.html) | [bwe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1687&db=1) |
| [ⲃⲱϣ](https://coptic-dictionary.org/entry.cgi?tla=C579) (ID:C579) |  | [bše](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1797&db=1) |
| [ⲃⲁϣⲟⲩϣ](https://coptic-dictionary.org/entry.cgi?tla=C593) (ID:C593) |  | [bšwše](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1800&db=1) |
| [ⲃⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C594) (ID:C594) | [bꜣḥ](https://oraec.github.io/corpus/53510.html) |  |
| [ⲃⲱⲱϩ](https://coptic-dictionary.org/entry.cgi?tla=C596) (ID:C596) |  | [Bẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1781&db=1) |
| [ⲃⲟⲩϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C597) (ID:C597) | [bhꜣ](https://oraec.github.io/corpus/56690.html) |  |
| [ⲃⲉϩⲃⲉϩ](https://coptic-dictionary.org/entry.cgi?tla=C599) (ID:C599) | [wḥwḥ](https://oraec.github.io/corpus/48980.html) | [wḥwḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-2140&db=1) |
| [ⲃⲁϩⲁⲗ](https://coptic-dictionary.org/entry.cgi?tla=C600) (ID:C600) | [Bꜥr](https://oraec.github.io/corpus/54960.html) | [Bꜥl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1683&db=1) |
| [ⲃⲱϩⲛ](https://coptic-dictionary.org/entry.cgi?tla=C602) (ID:C602) | [bhn](https://oraec.github.io/corpus/859161.html) |  |
| [ⲃⲱϩⲛ](https://coptic-dictionary.org/entry.cgi?tla=C603) (ID:C603) | [bhn](https://oraec.github.io/corpus/859161.html) |  |
| [ⲃⲁϩⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C604) (ID:C604) | [bḥz.t](https://oraec.github.io/corpus/56910.html) | [bḥs.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1775&db=1) |
| [ⲃⲱϩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C605) (ID:C605) |  | [bhṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1773&db=1) |
| [ⲃⲓϫⲓ](https://coptic-dictionary.org/entry.cgi?tla=C607) (ID:C607) | [bgꜣ](https://oraec.github.io/corpus/850481.html) | [bky](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1821&db=1) |
| [ⲃⲏϭ](https://coptic-dictionary.org/entry.cgi?tla=C610) (ID:C610) | [bjk](https://oraec.github.io/corpus/54680.html) | [byk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1807&db=1) |
| [ⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C615) (ID:C615) | [r](https://oraec.github.io/corpus/91900.html) | [r](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3338&db=1) |
| [ⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C616) (ID:C616) | [jw](https://oraec.github.io/corpus/21881.html) | [jw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-15&db=1) |
| [ⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C617) (ID:C617) | [j](https://oraec.github.io/corpus/20030.html) | [j](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=297&db=1) |
| [ⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C618) (ID:C618) | [jw](https://oraec.github.io/corpus/21881.html) | [j.jr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=305&db=1) |
| [ⲉⲣⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C619) (ID:C619) |  | [r](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-16&db=1) |
| [ⲉⲃⲏ](https://coptic-dictionary.org/entry.cgi?tla=C620) (ID:C620) | [bjꜣ.yt](https://oraec.github.io/corpus/54480.html) | [ꜣb.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=67&db=1) |
| [ⲉⲃⲓⲱ](https://coptic-dictionary.org/entry.cgi?tla=C624) (ID:C624) | [bj.t](https://oraec.github.io/corpus/54210.html) | [jby.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=441&db=1) |
| [ⲉⲃⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C627) (ID:C627) | [bj.tj](https://oraec.github.io/corpus/54230.html) | [jbyṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=443&db=1) |
| [ⲉⲃⲓⲏⲛ](https://coptic-dictionary.org/entry.cgi?tla=C628) (ID:C628) | [bjn](https://oraec.github.io/corpus/54610.html) | [ꜣbyn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=73&db=1) |
| [ⲉⲃⲓⲏⲛ](https://coptic-dictionary.org/entry.cgi?tla=C629) (ID:C629) | [bjn](https://oraec.github.io/corpus/54610.html) | [ꜣbyn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=73&db=1) |
| [ⲉⲃⲓⲏⲛ](https://coptic-dictionary.org/entry.cgi?tla=C630) (ID:C630) | [bjn](https://oraec.github.io/corpus/54605.html) | [byn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1646&db=1) |
| [ⲉⲃⲣⲁ](https://coptic-dictionary.org/entry.cgi?tla=C633) (ID:C633) | [pr.t](https://oraec.github.io/corpus/60310.html) | [pr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1989&db=1) |
| [ⲉⲃⲣⲏϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C636) (ID:C636) | [brq](https://oraec.github.io/corpus/56530.html) |  |
| [ⲉⲃⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C639) (ID:C639) | [ꜣbd](https://oraec.github.io/corpus/93.html) | [jbd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=446&db=1) |
| [ϩⲣⲉⲃⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C640) (ID:C640) |  | [ẖr-jbd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-5446&db=1) |
| [ⲉⲕⲓⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C641) (ID:C641) | [qꜣb.t](https://oraec.github.io/corpus/159290.html) |  |
| [ⲉⲗⲟⲓϩ](https://coptic-dictionary.org/entry.cgi?tla=C648) (ID:C648) | [jm.j-rʾ-jḥ.w](https://oraec.github.io/corpus/600270.html) | [mr-jḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2509&db=1) |
| [ⲉⲗⲕⲱ](https://coptic-dictionary.org/entry.cgi?tla=C649) (ID:C649) | [nqꜥ.wt](https://oraec.github.io/corpus/89040.html) | [ꜣlqw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=181&db=1) |
| [ⲉⲗⲟⲟⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C651) (ID:C651) | [jꜣrr.wt](https://oraec.github.io/corpus/20830.html) | [ꜣlly](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=179&db=1) |
| [ⲉⲗⲁⲙ](https://coptic-dictionary.org/entry.cgi?tla=C662) (ID:C662) | [ꜥnb.yt](https://oraec.github.io/corpus/38400.html) |  |
| [ⲉⲗⲧⲟϥ](https://coptic-dictionary.org/entry.cgi?tla=C663) (ID:C663) | [ntf](https://oraec.github.io/corpus/90030.html) |  |
| [ⲉⲙⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C667) (ID:C667) | [mjw.t](https://oraec.github.io/corpus/854443.html) | [my.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2326&db=1) |
| [ⲉⲙⲓⲙ](https://coptic-dictionary.org/entry.cgi?tla=C668) (ID:C668) | [ꜥmꜥm.w](https://oraec.github.io/corpus/37830.html) | [ꜥmꜥme](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=969&db=1) |
| [ⲉⲙⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C669) (ID:C669) | [jmn.tj](https://oraec.github.io/corpus/26151.html) | [jmnṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=520&db=1) |
| [ⲉⲙⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C670) (ID:C670) | [jmn.tj](https://oraec.github.io/corpus/26150.html) | [jmnṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=520&db=1) |
| [ⲉⲙⲛⲉⲩⲓ](https://coptic-dictionary.org/entry.cgi?tla=C671) (ID:C671) | [Mr-wr](https://oraec.github.io/corpus/72230.html) | [Mr-wr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2510&db=1) |
| [ⲉⲙⲏⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C672) (ID:C672) | [mr](https://oraec.github.io/corpus/71840.html) | [mꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2273&db=1) |
| [ⲉⲙⲓⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C673) (ID:C673) | [jms.t](https://oraec.github.io/corpus/26440.html) | [ꜣmys](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=105&db=1) |
| [ⲉⲙⲉϣϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C676) (ID:C676) | [jmskꜣ](https://oraec.github.io/corpus/26450.html) | [ꜣmsk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=112&db=1) |
| [ⲉⲛⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C677) (ID:C677) | [jn-jw](https://oraec.github.io/corpus/550032.html) | [jn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=527&db=1) |
| [ⲉⲛⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C678) (ID:C678) | [hꜣnꜣ](https://oraec.github.io/corpus/97660.html) | [hwn-nꜣ.w](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3721&db=1) |
| [ⲉⲛⲟⲩⲛⲅ](https://coptic-dictionary.org/entry.cgi?tla=C680) (ID:C680) | [jnnk](https://oraec.github.io/corpus/27520.html) | [ꜣnq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=128&db=1) |
| [ⲉⲛⲧ-](https://coptic-dictionary.org/entry.cgi?tla=C681) (ID:C681) | [n.tj](https://oraec.github.io/corpus/89850.html) | [nty](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3301&db=1) |
| [ⲉⲛϩ](https://coptic-dictionary.org/entry.cgi?tla=C682) (ID:C682) | [jnḥ](https://oraec.github.io/corpus/27700.html) | [jnḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=585&db=1) |
| [ⲉⲛⲉϩ](https://coptic-dictionary.org/entry.cgi?tla=C684) (ID:C684) | [nḥḥ](https://oraec.github.io/corpus/86570.html) | [nḥḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3237&db=1) |
| [ⲉⲛⲉϩ](https://coptic-dictionary.org/entry.cgi?tla=C685) (ID:C685) | [nḥḥ](https://oraec.github.io/corpus/86580.html) | [nḥḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3237&db=1) |
| [ⲉⲛⲉϩ](https://coptic-dictionary.org/entry.cgi?tla=C686) (ID:C686) | [nḥḥ](https://oraec.github.io/corpus/86580.html) | [nḥḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3237&db=1) |
| [ⲉⲡⲏⲡ](https://coptic-dictionary.org/entry.cgi?tla=C691) (ID:C691) | [Jpjp](https://oraec.github.io/corpus/24310.html) |  |
| [ⲉⲡⲣⲁ](https://coptic-dictionary.org/entry.cgi?tla=C692) (ID:C692) | [pr.t](https://oraec.github.io/corpus/60330.html) |  |
| [ⲉⲡϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C697) (ID:C697) | [ꜥpšꜣ.y](https://oraec.github.io/corpus/37210.html) |  |
| [ⲉⲣⲓ](https://coptic-dictionary.org/entry.cgi?tla=C699) (ID:C699) | [jr.yt](https://oraec.github.io/corpus/28610.html) |  |
| [ⲉⲣⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C708) (ID:C708) | [jrṯ.t](https://oraec.github.io/corpus/854491.html) | [jrte.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-2378&db=1) |
| [ⲉⲣⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C709) (ID:C709) | [jrṯ.t](https://oraec.github.io/corpus/854491.html) | [jrte.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-2378&db=1) |
| [ⲉⲣⲏⲩ](https://coptic-dictionary.org/entry.cgi?tla=C714) (ID:C714) | [jr.j](https://oraec.github.io/corpus/28510.html) | [jry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=632&db=1) |
| [ⲉⲣⲏⲩ](https://coptic-dictionary.org/entry.cgi?tla=C715) (ID:C715) | [jr.j](https://oraec.github.io/corpus/28510.html) | [jry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=632&db=1) |
| [ⲉⲣϣⲁⲛ](https://coptic-dictionary.org/entry.cgi?tla=C716) (ID:C716) | [zḫn](https://oraec.github.io/corpus/142460.html) | [jr-ḫn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=630&db=1) |
| [ⲉⲣϣⲓϣⲓ](https://coptic-dictionary.org/entry.cgi?tla=C718) (ID:C718) |  | [jr-sḫy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=619&db=1) |
| [ⲉⲥⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C725) (ID:C725) | [zꜣṯ.w](https://oraec.github.io/corpus/127650.html) | [ꜣsṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=228&db=1) |
| [ⲉⲥⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C734) (ID:C734) | [zr](https://oraec.github.io/corpus/138880.html) | [jsw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=700&db=1) |
| [ⲉⲥⲱ](https://coptic-dictionary.org/entry.cgi?tla=C735) (ID:C735) | [zr.t](https://oraec.github.io/corpus/138900.html) | [jsw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=700&db=1) |
| [ⲉⲧ-](https://coptic-dictionary.org/entry.cgi?tla=C737) (ID:C737) | [n.tj](https://oraec.github.io/corpus/89850.html) | [nty](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3301&db=1) |
| [ⲉⲁⲧ](https://coptic-dictionary.org/entry.cgi?tla=C738) (ID:C738) | [ꜥḏ](https://oraec.github.io/corpus/41960.html) | [ꜥt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1147&db=1) |
| [ⲉⲧⲃⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C739) (ID:C739) | [r-ḏbꜣ.t](https://oraec.github.io/corpus/851527.html) | [r-ḏbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3401&db=1) |
| [ⲉⲧⲏϣⲓ](https://coptic-dictionary.org/entry.cgi?tla=C747) (ID:C747) | [dšr](https://oraec.github.io/corpus/180680.html) |  |
| [ⲉⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C749) (ID:C749) | [jꜣ.w](https://oraec.github.io/corpus/20360.html) | [ꜣwy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=45&db=1) |
| [ⲉⲟⲩⲱ](https://coptic-dictionary.org/entry.cgi?tla=C755) (ID:C755) | [jwꜣ.yt](https://oraec.github.io/corpus/22230.html) | [jwy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=392&db=1) |
| [ⲉⲩⲛⲓ](https://coptic-dictionary.org/entry.cgi?tla=C762) (ID:C762) | [bnw.t](https://oraec.github.io/corpus/55650.html) |  |
| [ⲉⲫⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C763) (ID:C763) | [nfr-ḥtp](https://oraec.github.io/corpus/550400.html) | [Nfr-ḥtp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3178&db=1) |
| [ⲉⲫⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C764) (ID:C764) | [nfr-ḥtp](https://oraec.github.io/corpus/550400.html) | [Nfr-ḥtp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3178&db=1) |
| [ⲉϣⲟ](https://coptic-dictionary.org/entry.cgi?tla=C765) (ID:C765) | [sḫr](https://oraec.github.io/corpus/142820.html) |  |
| [ⲉϣⲱ](https://coptic-dictionary.org/entry.cgi?tla=C766) (ID:C766) | [sḫr](https://oraec.github.io/corpus/142820.html) |  |
| [ⲉϣⲱ](https://coptic-dictionary.org/entry.cgi?tla=C767) (ID:C767) | [šꜣj.t](https://oraec.github.io/corpus/151410.html) | [jše.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=708&db=1) |
| [ϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C768) (ID:C768) | [šꜣj](https://oraec.github.io/corpus/151350.html) | [šꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5806&db=1) |
| [ⲉϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C771) (ID:C771) | [jḥ](https://oraec.github.io/corpus/30410.html) | [jḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=666&db=1) |
| [ⲉϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C772) (ID:C772) | [jḥ](https://oraec.github.io/corpus/30410.html) | [jḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=666&db=1) |
| [ⲉϩⲱ](https://coptic-dictionary.org/entry.cgi?tla=C775) (ID:C775) | [ꜥḥ.t](https://oraec.github.io/corpus/39890.html) | [ꜥḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-6306&db=1) |
| [ⲉϭⲱϣ](https://coptic-dictionary.org/entry.cgi?tla=C777) (ID:C777) |  | [Jkš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=724&db=1) |
| [ⲉϭⲟϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C778) (ID:C778) |  | [jkšy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=725&db=1) |
| [ⲏⲓ](https://coptic-dictionary.org/entry.cgi?tla=C783) (ID:C783) |  | [ꜥ.wy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=806&db=1) |
| [ⲏⲓ](https://coptic-dictionary.org/entry.cgi?tla=C789) (ID:C789) | [ꜥ](https://oraec.github.io/corpus/34360.html) | [ꜥ.wy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=802&db=1) |
| [ⲏⲓ](https://coptic-dictionary.org/entry.cgi?tla=C790) (ID:C790) | [y](https://oraec.github.io/corpus/21250.html) | [j](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=297&db=1) |
| [ⲏⲛ](https://coptic-dictionary.org/entry.cgi?tla=C792) (ID:C792) | [jꜥnꜥ](https://oraec.github.io/corpus/850186.html) | [ꜥꜥny](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=886&db=1) |
| [ⲏⲣ](https://coptic-dictionary.org/entry.cgi?tla=C793) (ID:C793) | [jr.j](https://oraec.github.io/corpus/28510.html) | [jry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=632&db=1) |
| [ⲏⲣⲡ](https://coptic-dictionary.org/entry.cgi?tla=C794) (ID:C794) | [jrp](https://oraec.github.io/corpus/29740.html) | [jrp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=640&db=1) |
| [ⲏⲣⲡ](https://coptic-dictionary.org/entry.cgi?tla=C795) (ID:C795) | [jrp](https://oraec.github.io/corpus/29740.html) | [jrp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=640&db=1) |
| [ⲏⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C799) (ID:C799) | [Ꜣs.t](https://oraec.github.io/corpus/271.html) | [Ꜣs.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=209&db=1) |
| [ⲏⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C800) (ID:C800) | [ꜥ.t](https://oraec.github.io/corpus/854495.html) | [ꜥe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=796&db=1) |
| [ⲏϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C801) (ID:C801) | [jꜣq.t](https://oraec.github.io/corpus/20990.html) |  |
| [ⲑⲣⲁⲛ](https://coptic-dictionary.org/entry.cgi?tla=C814) (ID:C814) |  | [tren](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7366&db=1) |
| [ⲑⲉⲣϣ](https://coptic-dictionary.org/entry.cgi?tla=C815) (ID:C815) | [dšr](https://oraec.github.io/corpus/180740.html) |  |
| [ⲑⲁϥ⸗](https://coptic-dictionary.org/entry.cgi?tla=C820) (ID:C820) | [tfi̯](https://oraec.github.io/corpus/171780.html) | [tfy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7263&db=1) |
| [ⲓ](https://coptic-dictionary.org/entry.cgi?tla=C11278) (ID:C11278) | [=j](https://oraec.github.io/corpus/10030.html) | [=y](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=300&db=1) |
| [ⲉⲓ](https://coptic-dictionary.org/entry.cgi?tla=C825) (ID:C825) | [jwi̯](https://oraec.github.io/corpus/21930.html) | [jy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=338&db=1) |
| [ⲉⲓ](https://coptic-dictionary.org/entry.cgi?tla=C826) (ID:C826) | [jwi̯](https://oraec.github.io/corpus/21930.html) | [jy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=338&db=1) |
| [ⲉⲓ](https://coptic-dictionary.org/entry.cgi?tla=C827) (ID:C827) | [jwi̯](https://oraec.github.io/corpus/21930.html) | [jy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=338&db=1) |
| [ⲉⲓⲁ](https://coptic-dictionary.org/entry.cgi?tla=C854) (ID:C854) | [jꜥi̯](https://oraec.github.io/corpus/21550.html) | [yꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=749&db=1) |
| [ⲉⲓⲁ](https://coptic-dictionary.org/entry.cgi?tla=C855) (ID:C855) | [jr.t](https://oraec.github.io/corpus/28250.html) | [jr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=624&db=1) |
| [ⲉⲓⲉ](https://coptic-dictionary.org/entry.cgi?tla=C866) (ID:C866) | [jꜣ](https://oraec.github.io/corpus/20060.html) |  |
| [ⲉⲓⲉ](https://coptic-dictionary.org/entry.cgi?tla=C867) (ID:C867) | [jꜣ](https://oraec.github.io/corpus/20060.html) |  |
| [ⲉⲓⲉ](https://coptic-dictionary.org/entry.cgi?tla=C868) (ID:C868) | [jꜣ](https://oraec.github.io/corpus/20060.html) |  |
| [ⲉⲓⲉ](https://coptic-dictionary.org/entry.cgi?tla=C869) (ID:C869) | [jꜣ](https://oraec.github.io/corpus/20060.html) |  |
| [ⲉⲓⲉ](https://coptic-dictionary.org/entry.cgi?tla=C870) (ID:C870) | [jꜣ](https://oraec.github.io/corpus/20060.html) |  |
| [ⲉⲓⲱ](https://coptic-dictionary.org/entry.cgi?tla=C871) (ID:C871) | [jꜥi̯](https://oraec.github.io/corpus/21550.html) | [yꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=749&db=1) |
| [ⲉⲓⲱ](https://coptic-dictionary.org/entry.cgi?tla=C876) (ID:C876) | [jꜥꜣ](https://oraec.github.io/corpus/34840.html) | [ꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=826&db=1) |
| [ⲉⲓⲱ](https://coptic-dictionary.org/entry.cgi?tla=C877) (ID:C877) | [jꜥꜣ](https://oraec.github.io/corpus/34840.html) | [ꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=826&db=1) |
| [ⲉⲓⲃ](https://coptic-dictionary.org/entry.cgi?tla=C882) (ID:C882) | [ꜣb](https://oraec.github.io/corpus/10270.html) | [yb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=765&db=1) |
| [ⲉⲓⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C883) (ID:C883) | [jbi̯](https://oraec.github.io/corpus/23640.html) | [ꜣby](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=72&db=1) |
| [ⲉⲓⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C884) (ID:C884) | [jbi̯](https://oraec.github.io/corpus/23640.html) | [ꜣybe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=16&db=1) |
| [ⲉⲓⲁⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C886) (ID:C886) | [jꜣb](https://oraec.github.io/corpus/20520.html) | [yꜥby.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=755&db=1) |
| [ⲉⲓⲉⲃⲧ](https://coptic-dictionary.org/entry.cgi?tla=C887) (ID:C887) | [jꜣb.tj](https://oraec.github.io/corpus/20570.html) | [jꜣbṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=335&db=1) |
| [ⲉⲓⲉⲃⲧ](https://coptic-dictionary.org/entry.cgi?tla=C888) (ID:C888) | [jꜣb.tj](https://oraec.github.io/corpus/20570.html) | [jꜣbṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=335&db=1) |
| [ⲉⲓⲁⲗ](https://coptic-dictionary.org/entry.cgi?tla=C889) (ID:C889) |  | [yl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=777&db=1) |
| [ⲉⲓⲟⲩⲗ](https://coptic-dictionary.org/entry.cgi?tla=C890) (ID:C890) | [jjr](https://oraec.github.io/corpus/21420.html) | [ꜣywr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=15&db=1) |
| [ⲉⲓⲟⲩⲗ](https://coptic-dictionary.org/entry.cgi?tla=C891) (ID:C891) | [jjr](https://oraec.github.io/corpus/21420.html) | [ꜣywr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=15&db=1) |
| [ⲉⲓⲉⲗⲉⲗ](https://coptic-dictionary.org/entry.cgi?tla=C893) (ID:C893) |  | [yꜥl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=759&db=1) |
| [ⲓⲉⲗⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C894) (ID:C894) |  | [yꜥl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=759&db=1) |
| [ⲉⲓⲟⲙ](https://coptic-dictionary.org/entry.cgi?tla=C895) (ID:C895) | [ym](https://oraec.github.io/corpus/24730.html) | [ym](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=771&db=1) |
| [ⲉⲓⲟⲙ](https://coptic-dictionary.org/entry.cgi?tla=C896) (ID:C896) |  | [ym](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=772&db=1) |
| [ⲉⲓⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C897) (ID:C897) | [ꜥm](https://oraec.github.io/corpus/37500.html) | [ꜥm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=962&db=1) |
| [ⲉⲙⲓ](https://coptic-dictionary.org/entry.cgi?tla=C898) (ID:C898) |  | [ꜥmy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7923&db=1) |
| [ⲉⲓⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C905) (ID:C905) | [jni̯](https://oraec.github.io/corpus/26870.html) | [jn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-21&db=1) |
| [ⲉⲓⲛⲉ (ⲛ-)](https://coptic-dictionary.org/entry.cgi?tla=C928) (ID:C928) |  | [yn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=773&db=1) |
| [ⲉⲓⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C931) (ID:C931) | [jnj](https://oraec.github.io/corpus/26890.html) |  |
| [ⲉⲓⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C932) (ID:C932) | [ꜥn.t](https://oraec.github.io/corpus/38130.html) | [ꜥne.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=983&db=1) |
| [ⲉⲓⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C933) (ID:C933) | [ꜥn.t](https://oraec.github.io/corpus/38120.html) |  |
| [ⲉⲓⲟⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C934) (ID:C934) | [wpw.t](https://oraec.github.io/corpus/45750.html) | [wpe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1323&db=1) |
| [ⲉⲓⲟⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C942) (ID:C942) | [jp.t](https://oraec.github.io/corpus/24120.html) | [jpy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=465&db=1) |
| [ⲉⲓⲡⲛ](https://coptic-dictionary.org/entry.cgi?tla=C943) (ID:C943) | [jpn](https://oraec.github.io/corpus/24430.html) | [jpn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=470&db=1) |
| [ⲉⲓⲟⲟⲣ](https://coptic-dictionary.org/entry.cgi?tla=C944) (ID:C944) | [jtr.w](https://oraec.github.io/corpus/33370.html) | [yr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=774&db=1) |
| [ϫⲓⲟⲟⲣ](https://coptic-dictionary.org/entry.cgi?tla=C946) (ID:C946) |  | [ṯꜣy-yr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7573&db=1) |
| [ⲉⲓⲉⲣⲟ](https://coptic-dictionary.org/entry.cgi?tla=C950) (ID:C950) | [jtr.w-ꜥꜣ](https://oraec.github.io/corpus/33400.html) | [yr-ꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-5022&db=1) |
| [ⲉⲓⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C951) (ID:C951) | [jri̯](https://oraec.github.io/corpus/851809.html) | [jr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=592&db=1) |
| [ⲉⲓⲥ](https://coptic-dictionary.org/entry.cgi?tla=C978) (ID:C978) | [js](https://oraec.github.io/corpus/31130.html) | [ꜥs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1096&db=1) |
| [ⲉⲓⲥ](https://coptic-dictionary.org/entry.cgi?tla=C979) (ID:C979) | [js](https://oraec.github.io/corpus/31130.html) | [ꜥs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1096&db=1) |
| [ⲓⲱⲥ](https://coptic-dictionary.org/entry.cgi?tla=C988) (ID:C988) | [ꜣs](https://oraec.github.io/corpus/266.html) | [ys](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=782&db=1) |
| [ⲉⲓⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C992) (ID:C992) | [jtj](https://oraec.github.io/corpus/32820.html) | [jt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=727&db=1) |
| [ⲉⲓⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C993) (ID:C993) | [jtj](https://oraec.github.io/corpus/32820.html) | [jt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=727&db=1) |
| [ⲉⲓⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C998) (ID:C998) | [jt](https://oraec.github.io/corpus/32830.html) | [jt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=728&db=1) |
| [ⲉⲓⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C999) (ID:C999) | [jꜣd.t](https://oraec.github.io/corpus/21180.html) | [yꜥṱꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=762&db=1) |
| [ⲉⲓⲧⲛ](https://coptic-dictionary.org/entry.cgi?tla=C1001) (ID:C1001) | [jtn](https://oraec.github.io/corpus/33120.html) | [jtn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=739&db=1) |
| [ⲉⲓⲁⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C1005) (ID:C1005) | [ꜥꜣ.t](https://oraec.github.io/corpus/34920.html) | [ꜥꜣyw.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=851&db=1) |
| [ⲉⲓⲟⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1006) (ID:C1006) | [jwy](https://oraec.github.io/corpus/22270.html) | [yrwy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=776&db=1) |
| [ⲓϣ](https://coptic-dictionary.org/entry.cgi?tla=C1009) (ID:C1009) | [wzš.t](https://oraec.github.io/corpus/49970.html) | [wh̭h̭y](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7500&db=1) |
| [ⲉⲓϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1010) (ID:C1010) | [ꜥḫi̯](https://oraec.github.io/corpus/40570.html) | [ꜥḫy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1084&db=1) |
| [ⲉⲓϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1016) (ID:C1016) | [ꜥḫi̯](https://oraec.github.io/corpus/40570.html) | [ꜥḫy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1084&db=1) |
| [ⲓϧ](https://coptic-dictionary.org/entry.cgi?tla=C1028) (ID:C1028) | [ꜣḫ](https://oraec.github.io/corpus/203.html) | [jḫy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=676&db=1) |
| [ⲉⲓⲱϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1029) (ID:C1029) | [ꜣḥ.t](https://oraec.github.io/corpus/191.html) | [ꜣḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=191&db=1) |
| [ⲥⲧⲉⲓⲱϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1032) (ID:C1032) | [sṯꜣ.t-ꜣḥ.t](https://oraec.github.io/corpus/148880.html) |  |
| [ⲕ](https://coptic-dictionary.org/entry.cgi?tla=C1035) (ID:C1035) | [=k](https://oraec.github.io/corpus/10110.html) | [=k](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6496&db=1) |
| [ⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1037) (ID:C1037) | [ky](https://oraec.github.io/corpus/163760.html) | [ky](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6525&db=1) |
| [ⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1038) (ID:C1038) | [ky](https://oraec.github.io/corpus/163760.html) | [ky](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6525&db=1) |
| [ⲕⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C1039) (ID:C1039) | [ky](https://oraec.github.io/corpus/163760.html) | [ky](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6525&db=1) |
| [ⲕⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C1042) (ID:C1042) |  | [n-ge](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2933&db=1) |
| [ⲕⲏ](https://coptic-dictionary.org/entry.cgi?tla=C1046) (ID:C1046) | [ky](https://oraec.github.io/corpus/163760.html) | [ky](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6525&db=1) |
| [ⲕⲟ](https://coptic-dictionary.org/entry.cgi?tla=C1047) (ID:C1047) | [kꜣ](https://oraec.github.io/corpus/162930.html) | [kꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6508&db=1) |
| [ⲕⲟⲓⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1050) (ID:C1050) | [qꜣ.yt](https://oraec.github.io/corpus/159160.html) | [qy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6259&db=1) |
| [ⲕⲟⲩⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1054) (ID:C1054) | [gꜣu̯](https://oraec.github.io/corpus/166210.html) | [gwy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6747&db=1) |
| [ⲕⲱ](https://coptic-dictionary.org/entry.cgi?tla=C1058) (ID:C1058) | [ḫꜣꜥ](https://oraec.github.io/corpus/113560.html) | [ḫꜣꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4386&db=1) |
| [ⲕⲏ](https://coptic-dictionary.org/entry.cgi?tla=C1059) (ID:C1059) | [ḫꜣꜥ](https://oraec.github.io/corpus/113560.html) | [ḫꜣꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4386&db=1) |
| [ⲕⲱ](https://coptic-dictionary.org/entry.cgi?tla=C1092) (ID:C1092) | [kꜣr](https://oraec.github.io/corpus/163620.html) | [qꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6514&db=1) |
| [ⲕⲱⲃ](https://coptic-dictionary.org/entry.cgi?tla=C1094) (ID:C1094) | [qꜣb](https://oraec.github.io/corpus/854562.html) | [qb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6287&db=1) |
| [ⲕⲱⲃ](https://coptic-dictionary.org/entry.cgi?tla=C1095) (ID:C1095) | [qꜣb](https://oraec.github.io/corpus/159260.html) |  |
| [ⲕⲏⲃⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1102) (ID:C1102) | [qby](https://oraec.github.io/corpus/160130.html) | [qbꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6294&db=1) |
| [ⲕⲱⲱⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1104) (ID:C1104) | [kfꜥ](https://oraec.github.io/corpus/164220.html) | [qby](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6297&db=1) |
| [ⲕⲃⲁ](https://coptic-dictionary.org/entry.cgi?tla=C1105) (ID:C1105) |  | [qbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6291&db=1) |
| [ⲕⲃⲁ](https://coptic-dictionary.org/entry.cgi?tla=C1107) (ID:C1107) |  | [qbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6291&db=1) |
| [ⲕⲃⲟ](https://coptic-dictionary.org/entry.cgi?tla=C1112) (ID:C1112) | [qbb](https://oraec.github.io/corpus/160170.html) | [qby](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-5933&db=1) |
| [ⲕⲃⲟ](https://coptic-dictionary.org/entry.cgi?tla=C1113) (ID:C1113) | [qbb](https://oraec.github.io/corpus/160180.html) | [qbꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6299&db=1) |
| [ⲕⲃⲱⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C1116) (ID:C1116) | [qbb](https://oraec.github.io/corpus/160190.html) | [qbb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6301&db=1) |
| [ⲕⲱⲃϩ](https://coptic-dictionary.org/entry.cgi?tla=C1117) (ID:C1117) | [qbḥ](https://oraec.github.io/corpus/160230.html) | [qbḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6309&db=1) |
| [ⲕⲟⲩⲕ](https://coptic-dictionary.org/entry.cgi?tla=C1119) (ID:C1119) |  | [qwqy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6284&db=1) |
| [ⲕⲟⲩⲕ](https://coptic-dictionary.org/entry.cgi?tla=C1121) (ID:C1121) | [qq](https://oraec.github.io/corpus/162280.html) | [kwk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6546&db=1) |
| [ⲕⲱⲕ](https://coptic-dictionary.org/entry.cgi?tla=C1122) (ID:C1122) |  | [qq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6471&db=1) |
| [ⲕⲁⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1129) (ID:C1129) | [kk.w](https://oraec.github.io/corpus/165680.html) | [kky](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6664&db=1) |
| [ⲕⲁⲕⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1131) (ID:C1131) | [qꜣꜥ.w](https://oraec.github.io/corpus/159210.html) |  |
| [ⲕⲁⲕⲟⲩⲡⲁⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1137) (ID:C1137) |  | [qqpt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6474&db=1) |
| [ⲕⲁⲕⲟⲩⲡⲁⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1138) (ID:C1138) |  | [qqpt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6474&db=1) |
| [ⲕⲗⲏ](https://coptic-dictionary.org/entry.cgi?tla=C1142) (ID:C1142) |  | [qle.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6417&db=1) |
| [ⲕⲁⲗⲏ](https://coptic-dictionary.org/entry.cgi?tla=C1143) (ID:C1143) |  | [qle.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6417&db=1) |
| [ⲕⲗⲟ](https://coptic-dictionary.org/entry.cgi?tla=C1144) (ID:C1144) |  | [krꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6604&db=1) |
| [ⲕⲗⲁⲗ](https://coptic-dictionary.org/entry.cgi?tla=C1154) (ID:C1154) |  | [qll](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6431&db=1) |
| [ⲕⲗⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1156) (ID:C1156) | [qꜣr.t](https://oraec.github.io/corpus/159380.html) | [qlꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6418&db=1) |
| [ⲕⲗⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1157) (ID:C1157) | [qꜣr.t](https://oraec.github.io/corpus/159380.html) | [qrr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6613&db=1) |
| [ⲕⲉⲗⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1158) (ID:C1158) | [qꜣr.t](https://oraec.github.io/corpus/159380.html) | [qlꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6418&db=1) |
| [ⲕⲉⲗⲱⲗ](https://coptic-dictionary.org/entry.cgi?tla=C1162) (ID:C1162) | [krr](https://oraec.github.io/corpus/165080.html) | [krl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6615&db=1) |
| [ⲕⲗⲟⲟⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1165) (ID:C1165) | [qrr](https://oraec.github.io/corpus/161770.html) | [qlꜥl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6421&db=1) |
| [ⲕⲗⲟⲙ](https://coptic-dictionary.org/entry.cgi?tla=C1173) (ID:C1173) |  | [qlm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6427&db=1) |
| [ⲕⲗⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1179) (ID:C1179) |  | [qlme.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6428&db=1) |
| [ⲕⲗⲯ](https://coptic-dictionary.org/entry.cgi?tla=C1189) (ID:C1189) |  | [qlps](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6425&db=1) |
| [ⲕⲉⲗϥⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1195) (ID:C1195) | [qrf.w](https://oraec.github.io/corpus/161730.html) |  |
| [ⲕⲗⲁϥⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1196) (ID:C1196) | [qrf.t](https://oraec.github.io/corpus/161710.html) | [qrft](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6396&db=1) |
| [ⲕⲱⲗϩ](https://coptic-dictionary.org/entry.cgi?tla=C1197) (ID:C1197) |  | [qlhe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6435&db=1) |
| [ⲕⲱⲗϩ](https://coptic-dictionary.org/entry.cgi?tla=C1204) (ID:C1204) |  | [qrḥy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-779&db=1) |
| [ⲕⲗϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1205) (ID:C1205) |  | [qrḥy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-779&db=1) |
| [ⲕⲱⲗϫ](https://coptic-dictionary.org/entry.cgi?tla=C1207) (ID:C1207) |  | [klḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6642&db=1) |
| [ⲕⲁⲙ](https://coptic-dictionary.org/entry.cgi?tla=C1213) (ID:C1213) | [qmꜣ](https://oraec.github.io/corpus/160630.html) | [qmꜣe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6331&db=1) |
| [ⲕⲓⲙ](https://coptic-dictionary.org/entry.cgi?tla=C1215) (ID:C1215) | [qmꜣ](https://oraec.github.io/corpus/854564.html) | [qmꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6327&db=1) |
| [ⲕⲙⲕⲙ](https://coptic-dictionary.org/entry.cgi?tla=C1223) (ID:C1223) | [qmqm](https://oraec.github.io/corpus/160850.html) | [qmqm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6343&db=1) |
| [ⲕⲙⲟⲙ](https://coptic-dictionary.org/entry.cgi?tla=C1225) (ID:C1225) | [kmm](https://oraec.github.io/corpus/164310.html) | [km](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1514&db=1) |
| [ⲕⲁⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1227) (ID:C1227) | [km](https://oraec.github.io/corpus/401218.html) | [km](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6579&db=1) |
| [ⲕⲁⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1228) (ID:C1228) | [km.y](https://oraec.github.io/corpus/164560.html) |  |
| [ⲕⲁⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1229) (ID:C1229) | [km.y](https://oraec.github.io/corpus/164560.html) |  |
| [ⲕⲏⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1232) (ID:C1232) | [Km.t](https://oraec.github.io/corpus/164430.html) | [Kmy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6581&db=1) |
| [ⲕⲙⲏⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1236) (ID:C1236) |  | [kmeme.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6583&db=1) |
| [ⲕⲟⲙⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1237) (ID:C1237) | [qmy.t](https://oraec.github.io/corpus/160800.html) | [qmy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6338&db=1) |
| [ⲕⲏⲛ](https://coptic-dictionary.org/entry.cgi?tla=C1243) (ID:C1243) | [qn](https://oraec.github.io/corpus/160990.html) | [qne](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6346&db=1) |
| [ⲕⲟⲩⲛ⸗](https://coptic-dictionary.org/entry.cgi?tla=C1246) (ID:C1246) | [qnj](https://oraec.github.io/corpus/161180.html) | [qne](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6353&db=1) |
| [ⲕⲛⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1248) (ID:C1248) | [qni̯](https://oraec.github.io/corpus/160890.html) |  |
| [ⲕⲱⲛⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1253) (ID:C1253) |  | [qns](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6372&db=1) |
| [ⲕⲛⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1258) (ID:C1258) |  | [qnṱe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6379&db=1) |
| [ⲕⲛⲁⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C1261) (ID:C1261) | [qnj](https://oraec.github.io/corpus/161300.html) |  |
| [ⲕⲟⲛϥ](https://coptic-dictionary.org/entry.cgi?tla=C1265) (ID:C1265) | [qfn.y](https://oraec.github.io/corpus/160510.html) |  |
| [ⲕⲁⲛⲟⲩϥⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1266) (ID:C1266) | [šnf.t](https://oraec.github.io/corpus/156140.html) | [ḫnfy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4526&db=1) |
| [ⲕⲛϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1268) (ID:C1268) |  | [qnḥy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6371&db=1) |
| [ⲕⲟⲩⲛϫⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C1270) (ID:C1270) |  | [qnḏwꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6383&db=1) |
| [ⲕⲱⲡ](https://coptic-dictionary.org/entry.cgi?tla=C1276) (ID:C1276) | [kꜣp](https://oraec.github.io/corpus/854567.html) | [qpe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6316&db=1) |
| [ⲕⲏⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1282) (ID:C1282) | [kꜣp.t](https://oraec.github.io/corpus/163420.html) | [qpe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6318&db=1) |
| [ⲕⲟⲩⲡⲣ](https://coptic-dictionary.org/entry.cgi?tla=C1283) (ID:C1283) |  | [qwpre](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6275&db=1) |
| [ⲕⲟⲩⲣ](https://coptic-dictionary.org/entry.cgi?tla=C1291) (ID:C1291) |  | [qwr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1413&db=1) |
| [ⲕⲣⲟ](https://coptic-dictionary.org/entry.cgi?tla=C1293) (ID:C1293) |  | [qr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6384&db=1) |
| [ⲕⲣⲱⲙ](https://coptic-dictionary.org/entry.cgi?tla=C1302) (ID:C1302) |  | [qrm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6397&db=1) |
| [ⲕⲱⲣⲙ](https://coptic-dictionary.org/entry.cgi?tla=C1308) (ID:C1308) |  | [qrm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6397&db=1) |
| [ⲕⲣⲙⲣⲙ](https://coptic-dictionary.org/entry.cgi?tla=C1309) (ID:C1309) |  | [qrmrme](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6399&db=1) |
| [ⲕⲣⲙⲧⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1315) (ID:C1315) |  | [qrmṱ=s](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6400&db=1) |
| [ⲭⲣⲉⲙⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1317) (ID:C1317) |  | [qrm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6397&db=1) |
| [ⲕⲣⲙⲉⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1318) (ID:C1318) |  | [qrm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6397&db=1) |
| [ⲕⲣⲙⲉⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1319) (ID:C1319) |  | [qrm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6397&db=1) |
| [ⲕⲣⲟⲩⲣ](https://coptic-dictionary.org/entry.cgi?tla=C1323) (ID:C1323) |  | [qrr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6402&db=1) |
| [ⲕⲁⲣⲟⲩⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1327) (ID:C1327) |  | [qrs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6407&db=1) |
| [ⲕⲱⲣϣ](https://coptic-dictionary.org/entry.cgi?tla=C1330) (ID:C1330) |  | [qrš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6408&db=1) |
| [ⲕⲱⲣϣ](https://coptic-dictionary.org/entry.cgi?tla=C1331) (ID:C1331) |  | [qrš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7953&db=1) |
| [ⲕⲱⲣϥ](https://coptic-dictionary.org/entry.cgi?tla=C1336) (ID:C1336) | [krp](https://oraec.github.io/corpus/165060.html) | [grp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7578&db=1) |
| [ⲕⲣⲟϥ](https://coptic-dictionary.org/entry.cgi?tla=C1340) (ID:C1340) | [qrf](https://oraec.github.io/corpus/161690.html) | [qrf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6395&db=1) |
| [ⲕⲁⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1358) (ID:C1358) | [qs](https://oraec.github.io/corpus/162200.html) | [qs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6458&db=1) |
| [ⲕⲁⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1363) (ID:C1363) | [qs](https://oraec.github.io/corpus/162200.html) | [qs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6458&db=1) |
| [ⲕⲁⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1364) (ID:C1364) | [qs](https://oraec.github.io/corpus/162200.html) | [qs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6458&db=1) |
| [ⲕⲟⲉⲓⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1365) (ID:C1365) |  | [gys](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6710&db=1) |
| [ⲕⲱⲱⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1366) (ID:C1366) | [qrs](https://oraec.github.io/corpus/161940.html) | [qs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6451&db=1) |
| [ⲕⲱⲱⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1367) (ID:C1367) | [qrs](https://oraec.github.io/corpus/161950.html) | [qs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4718&db=1) |
| [ⲕⲱⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1368) (ID:C1368) | [qrs](https://oraec.github.io/corpus/161950.html) | [qs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4718&db=1) |
| [ⲕⲁⲓⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1373) (ID:C1373) | [qrs.t](https://oraec.github.io/corpus/161960.html) | [qs.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6459&db=1) |
| [ⲕⲁⲥⲕⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1376) (ID:C1376) |  | [qsqs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6465&db=1) |
| [ⲕⲟⲥⲕⲥ ⲉⲃⲟⲗ](https://coptic-dictionary.org/entry.cgi?tla=C1379) (ID:C1379) | [ksks](https://oraec.github.io/corpus/165520.html) | [gsgs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6939&db=1) |
| [ⲝⲟⲩⲣ](https://coptic-dictionary.org/entry.cgi?tla=C1380) (ID:C1380) |  | [kswr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6651&db=1) |
| [ⲕⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1383) (ID:C1383) | [qd](https://oraec.github.io/corpus/162420.html) | [qd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6475&db=1) |
| [ⲕⲱⲧ (ⲉⲃⲟⲗ)](https://coptic-dictionary.org/entry.cgi?tla=C1384) (ID:C1384) | [qd](https://oraec.github.io/corpus/162420.html) | [qd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6475&db=1) |
| [ⲉⲕⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1391) (ID:C1391) | [qd.w](https://oraec.github.io/corpus/162500.html) | [qd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6477&db=1) |
| [ⲕⲓⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1411) (ID:C1411) | [qd.t](https://oraec.github.io/corpus/162490.html) | [qd.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6478&db=1) |
| [ⲕⲓⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1413) (ID:C1413) | [qd.t](https://oraec.github.io/corpus/162470.html) | [qdy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6483&db=1) |
| [ⲕⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1416) (ID:C1416) | [qdi̯](https://oraec.github.io/corpus/162530.html) | [qdy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6485&db=1) |
| [ⲕⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1431) (ID:C1431) | [qd](https://oraec.github.io/corpus/162440.html) | [qdy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-873&db=1) |
| [ⲕⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1437) (ID:C1437) | [qd](https://oraec.github.io/corpus/162440.html) | [qdy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-873&db=1) |
| [ⲕⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1442) (ID:C1442) | [qd](https://oraec.github.io/corpus/162440.html) | [qdy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-873&db=1) |
| [ⲕⲧⲟ](https://coptic-dictionary.org/entry.cgi?tla=C1451) (ID:C1451) | [qdi̯](https://oraec.github.io/corpus/162530.html) | [qdy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6485&db=1) |
| [ⲕⲱⲧϥ](https://coptic-dictionary.org/entry.cgi?tla=C1467) (ID:C1467) | [qdf](https://oraec.github.io/corpus/162580.html) | [qtf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6491&db=1) |
| [ⲕⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C1473) (ID:C1473) | [qꜣw](https://oraec.github.io/corpus/159010.html) | [qy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7839&db=1) |
| [ⲕⲁϣ](https://coptic-dictionary.org/entry.cgi?tla=C1478) (ID:C1478) | [gꜣš](https://oraec.github.io/corpus/166570.html) | [qše](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6466&db=1) |
| [ⲕⲁϣ](https://coptic-dictionary.org/entry.cgi?tla=C1479) (ID:C1479) | [gꜣš](https://oraec.github.io/corpus/166570.html) | [qše](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6466&db=1) |
| [ⲕⲏϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1484) (ID:C1484) | [qꜥḥ](https://oraec.github.io/corpus/159900.html) |  |
| [ⲕⲱⲱϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1485) (ID:C1485) |  | [ḫrš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4576&db=1) |
| [ⲕⲁϣⲁⲃⲉⲗ](https://coptic-dictionary.org/entry.cgi?tla=C1487) (ID:C1487) |  | [qšbl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6469&db=1) |
| [ⲕⲟⲩϣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1490) (ID:C1490) |  | [qwšṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6281&db=1) |
| [ⲕⲁϥ](https://coptic-dictionary.org/entry.cgi?tla=C1492) (ID:C1492) | [kfꜣ](https://oraec.github.io/corpus/164120.html) |  |
| [ⲕⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C1494) (ID:C1494) | [qꜣḥ](https://oraec.github.io/corpus/159410.html) | [qh](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6439&db=1) |
| [ⲕⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C1495) (ID:C1495) | [qꜥḥ.t](https://oraec.github.io/corpus/159920.html) | [qḥy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6445&db=1) |
| [ⲕⲉϩ](https://coptic-dictionary.org/entry.cgi?tla=C1501) (ID:C1501) | [qꜥḥ](https://oraec.github.io/corpus/159830.html) |  |
| [ⲕⲟⲉⲓϩ](https://coptic-dictionary.org/entry.cgi?tla=C1503) (ID:C1503) | [qꜥḥ.w](https://oraec.github.io/corpus/159840.html) | [qḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6443&db=1) |
| [ⲕⲟⲟϩ](https://coptic-dictionary.org/entry.cgi?tla=C1504) (ID:C1504) | [qꜥḥ.w](https://oraec.github.io/corpus/159840.html) | [qḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6443&db=1) |
| [ⲕⲟⲟϩ](https://coptic-dictionary.org/entry.cgi?tla=C1505) (ID:C1505) | [qꜥḥ.w](https://oraec.github.io/corpus/159840.html) | [qḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6443&db=1) |
| [ⲕⲱϩ](https://coptic-dictionary.org/entry.cgi?tla=C1507) (ID:C1507) | [khꜣ](https://oraec.github.io/corpus/854569.html) |  |
| [ⲕⲟⲓⲁϩⲕ](https://coptic-dictionary.org/entry.cgi?tla=C1522) (ID:C1522) | [Kꜣ-ḥr-kꜣ](https://oraec.github.io/corpus/163150.html) |  |
| [ⲕⲱϩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1524) (ID:C1524) | [qhd](https://oraec.github.io/corpus/858172.html) |  |
| [ⲕⲉϩⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1529) (ID:C1529) | [qꜥḥ.t](https://oraec.github.io/corpus/159910.html) | [qh.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6442&db=1) |
| [ⲕⲁϫⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1533) (ID:C1533) | [kṯ](https://oraec.github.io/corpus/165930.html) |  |
| [ⲗⲁ](https://coptic-dictionary.org/entry.cgi?tla=C1537) (ID:C1537) |  | [rꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3434&db=1) |
| [ⲗⲟ](https://coptic-dictionary.org/entry.cgi?tla=C1547) (ID:C1547) | [rwi̯](https://oraec.github.io/corpus/93540.html) | [lꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-6562&db=1) |
| [ⲗⲁⲃⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1561) (ID:C1561) | [rw-ꜣbw](https://oraec.github.io/corpus/93500.html) | [lby.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3660&db=1) |
| [ⲗⲓⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1562) (ID:C1562) | [npꜣ](https://oraec.github.io/corpus/854651.html) | [lby](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3658&db=1) |
| [ⲗⲓⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1572) (ID:C1572) | [npꜣ](https://oraec.github.io/corpus/854651.html) | [lby](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3658&db=1) |
| [ⲗⲱⲃϣ](https://coptic-dictionary.org/entry.cgi?tla=C1588) (ID:C1588) | [nwḫ](https://oraec.github.io/corpus/81460.html) |  |
| [ⲗⲱⲃϣ](https://coptic-dictionary.org/entry.cgi?tla=C1591) (ID:C1591) | [bnš](https://oraec.github.io/corpus/56120.html) |  |
| [ⲗⲟⲕ](https://coptic-dictionary.org/entry.cgi?tla=C1594) (ID:C1594) |  | [lq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3698&db=1) |
| [ⲗⲁⲕⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1609) (ID:C1609) |  | [lqnṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3704&db=1) |
| [ⲗⲁⲕⲉⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1610) (ID:C1610) |  | [lqnṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3704&db=1) |
| [ⲗⲱⲕⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1612) (ID:C1612) | [nsq](https://oraec.github.io/corpus/88370.html) | [lks](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3709&db=1) |
| [ⲗⲁⲕⲥⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1619) (ID:C1619) | [krs](https://oraec.github.io/corpus/165110.html) |  |
| [ⲗⲏⲗ](https://coptic-dictionary.org/entry.cgi?tla=C1629) (ID:C1629) | [rr](https://oraec.github.io/corpus/95270.html) | [rl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-698&db=1) |
| [ⲗⲁⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1631) (ID:C1631) | [ꜥrꜥr](https://oraec.github.io/corpus/39360.html) | [ꜥrꜥr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1029&db=1) |
| [ⲗⲉⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1632) (ID:C1632) |  | [lwlw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3648&db=1) |
| [ⲗⲉⲗⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C1637) (ID:C1637) | [nn.w](https://oraec.github.io/corpus/84560.html) | [nn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3190&db=1) |
| [ⲗⲉⲗⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C1638) (ID:C1638) | [nn.w](https://oraec.github.io/corpus/84560.html) | [nn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3190&db=1) |
| [ⲗⲟⲩⲗⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1640) (ID:C1640) |  | [lylꜥy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-646&db=1) |
| [ⲗⲉⲙⲏⲏϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1669) (ID:C1669) | [jm.j-rʾ-mšꜥ](https://oraec.github.io/corpus/400043.html) | [mr-mšꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2517&db=1) |
| [ⲗⲁⲙϫⲁⲧⲡ](https://coptic-dictionary.org/entry.cgi?tla=C1670) (ID:C1670) |  | [lnḏpꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3672&db=1) |
| [ⲗⲁⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C1672) (ID:C1672) |  | [lyn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3628&db=1) |
| [ⲗⲉⲟⲛ](https://coptic-dictionary.org/entry.cgi?tla=C1673) (ID:C1673) |  | [lꜣn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3621&db=1) |
| [ⲗⲉⲯⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1679) (ID:C1679) | [nzp.w](https://oraec.github.io/corpus/88180.html) |  |
| [ⲗⲁⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1684) (ID:C1684) | [ns](https://oraec.github.io/corpus/87800.html) | [ls](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3694&db=1) |
| [ⲗⲱⲱⲥ](https://coptic-dictionary.org/entry.cgi?tla=C1697) (ID:C1697) | [nss](https://oraec.github.io/corpus/88350.html) |  |
| [ⲗⲁϣⲓⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1724) (ID:C1724) |  | [rẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-6690&db=1) |
| [ⲗⲁϣⲁⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1725) (ID:C1725) |  | [mr-šn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2527&db=1) |
| [ⲗⲱⲱϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1730) (ID:C1730) |  | [rfꜥy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3480&db=1) |
| [ⲗⲁϧⲉⲙ](https://coptic-dictionary.org/entry.cgi?tla=C1735) (ID:C1735) | [ꜥẖm.w](https://oraec.github.io/corpus/40830.html) | [ꜥḫm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4227&db=1) |
| [ⲗⲉϩ](https://coptic-dictionary.org/entry.cgi?tla=C1737) (ID:C1737) | [nh.w](https://oraec.github.io/corpus/85420.html) | [lh](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3680&db=1) |
| [ⲗϩⲱⲃ](https://coptic-dictionary.org/entry.cgi?tla=C1742) (ID:C1742) | [rhb](https://oraec.github.io/corpus/95420.html) | [lhb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3682&db=1) |
| [ⲗⲱϩⲙ](https://coptic-dictionary.org/entry.cgi?tla=C1746) (ID:C1746) |  | [lẖm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3693&db=1) |
| [ⲗϩⲏⲙ](https://coptic-dictionary.org/entry.cgi?tla=C1748) (ID:C1748) | [nhm](https://oraec.github.io/corpus/85580.html) | [nhm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3221&db=1) |
| [ⲗⲟϫⲗϫ](https://coptic-dictionary.org/entry.cgi?tla=C1760) (ID:C1760) |  | [lḏlḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3717&db=1) |
| [ⲗⲱϫϩ](https://coptic-dictionary.org/entry.cgi?tla=C1765) (ID:C1765) |  | [lkḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3708&db=1) |
| [ⲗⲟϭ](https://coptic-dictionary.org/entry.cgi?tla=C1767) (ID:C1767) |  | [rẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-6690&db=1) |
| [ⲗⲁϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C11283) (ID:C11283) | [rqi̯](https://oraec.github.io/corpus/96290.html) | [lgy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3710&db=1) |
| [ⲙⲁ](https://coptic-dictionary.org/entry.cgi?tla=C1771) (ID:C1771) | [mꜣꜥ](https://oraec.github.io/corpus/850060.html) | [mꜣꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2291&db=1) |
| [ⲙⲁ-](https://coptic-dictionary.org/entry.cgi?tla=C1781) (ID:C1781) | [jmi̯](https://oraec.github.io/corpus/851706.html) | [my](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2324&db=1) |
| [ⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1785) (ID:C1785) | [mri̯](https://oraec.github.io/corpus/72470.html) | [mr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2496&db=1) |
| [ⲙⲉⲣⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1788) (ID:C1788) | [mrw.tj](https://oraec.github.io/corpus/72660.html) | [mrṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2534&db=1) |
| [ⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1789) (ID:C1789) | [mꜣꜥ.t](https://oraec.github.io/corpus/66620.html) | [mꜣꜥ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2297&db=1) |
| [ⲙⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1800) (ID:C1800) | [mtj](https://oraec.github.io/corpus/77420.html) | [mtry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2797&db=1) |
| [ⲙⲏ](https://coptic-dictionary.org/entry.cgi?tla=C1801) (ID:C1801) | [mw.yt](https://oraec.github.io/corpus/69240.html) | [mꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2277&db=1) |
| [ⲙⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C1809) (ID:C1809) | [mwt](https://oraec.github.io/corpus/69300.html) | [mwt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2408&db=1) |
| [ⲙⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C1810) (ID:C1810) | [mwt](https://oraec.github.io/corpus/69310.html) | [mwt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-762&db=1) |
| [ⲣⲉϥⲙⲟⲟⲩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1813) (ID:C1813) |  | [rmṯ-jw=f-mwt.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4367&db=1) |
| [ⲙⲟⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1819) (ID:C1819) | [mꜣw.t](https://oraec.github.io/corpus/66870.html) | [mꜣwy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-2421&db=1) |
| [ⲙⲟⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1822) (ID:C1822) | [mꜣw.t](https://oraec.github.io/corpus/66830.html) | [mꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2283&db=1) |
| [ⲙⲟⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1823) (ID:C1823) | [mꜣw.t](https://oraec.github.io/corpus/66830.html) | [mꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2283&db=1) |
| [ⲙⲟⲩⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1824) (ID:C1824) | [mꜣw](https://oraec.github.io/corpus/66150.html) | [mꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2279&db=1) |
| [ⲙⲟⲩⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1825) (ID:C1825) | [mꜣj](https://oraec.github.io/corpus/66370.html) | [mꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2281&db=1) |
| [ⲙⲟⲩⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1826) (ID:C1826) | [mꜣj](https://oraec.github.io/corpus/66370.html) | [mꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2281&db=1) |
| [ⲙⲟⲩⲓⲏ](https://coptic-dictionary.org/entry.cgi?tla=C1827) (ID:C1827) | [mꜣj.t](https://oraec.github.io/corpus/66420.html) | [mꜣw.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2302&db=1) |
| [ⲙⲁⲁⲃ](https://coptic-dictionary.org/entry.cgi?tla=C1830) (ID:C1830) | [mꜥbꜣ](https://oraec.github.io/corpus/68690.html) |  |
| [ⲙⲟⲩⲕⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1841) (ID:C1841) | [mꜣq.t](https://oraec.github.io/corpus/67450.html) | [mqy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2724&db=1) |
| [ⲙⲟⲕⲙⲉⲕ](https://coptic-dictionary.org/entry.cgi?tla=C1842) (ID:C1842) | [mqmq](https://oraec.github.io/corpus/76660.html) | [mqmq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2717&db=1) |
| [ⲙⲟⲕⲙⲉⲕ](https://coptic-dictionary.org/entry.cgi?tla=C1843) (ID:C1843) |  | [mqmq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7743&db=1) |
| [ⲙⲁⲕⲣⲟ](https://coptic-dictionary.org/entry.cgi?tla=C1847) (ID:C1847) | [mqr](https://oraec.github.io/corpus/76710.html) |  |
| [ⲙⲁⲕϩ](https://coptic-dictionary.org/entry.cgi?tla=C1852) (ID:C1852) | [mkḥꜣ](https://oraec.github.io/corpus/77100.html) | [mqḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2721&db=1) |
| [ⲙⲟⲩⲕϩ](https://coptic-dictionary.org/entry.cgi?tla=C1856) (ID:C1856) |  | [mqḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2720&db=1) |
| [ⲙⲕⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C1857) (ID:C1857) |  | [mqḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2720&db=1) |
| [ⲙⲕⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C1858) (ID:C1858) |  | [mqḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7744&db=1) |
| [ⲙⲓⲟⲗⲱⲛ](https://coptic-dictionary.org/entry.cgi?tla=C1870) (ID:C1870) | [mnnn](https://oraec.github.io/corpus/70810.html) |  |
| [ⲙⲉⲗⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1872) (ID:C1872) |  | [mylṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2340&db=1) |
| [ⲙⲗⲁϧ](https://coptic-dictionary.org/entry.cgi?tla=C1874) (ID:C1874) |  | [mlẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-652&db=1) |
| [ⲙⲗⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C1875) (ID:C1875) |  | [mlẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2580&db=1) |
| [ⲙⲟⲩⲗϩ](https://coptic-dictionary.org/entry.cgi?tla=C1882) (ID:C1882) | [mnḥ](https://oraec.github.io/corpus/70920.html) | [mnḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2466&db=1) |
| [ⲙⲟⲩⲗⲁϫ](https://coptic-dictionary.org/entry.cgi?tla=C1886) (ID:C1886) |  | [ꜣmwlḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=109&db=1) |
| [ⲙⲟⲩⲗϫ](https://coptic-dictionary.org/entry.cgi?tla=C1887) (ID:C1887) | [knm](https://oraec.github.io/corpus/164780.html) |  |
| [ⲙⲙⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C1890) (ID:C1890) | [mn](https://oraec.github.io/corpus/69560.html) | [mn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2418&db=1) |
| [ⲙⲛⲧⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C1891) (ID:C1891) |  | [mn-mtw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2436&db=1) |
| [ⲙⲁⲛ](https://coptic-dictionary.org/entry.cgi?tla=C1900) (ID:C1900) | [mn](https://oraec.github.io/corpus/69610.html) | [mn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2419&db=1) |
| [ⲙⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C1901) (ID:C1901) | [jrm](https://oraec.github.io/corpus/29840.html) | [jrm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=646&db=1) |
| [ⲙⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C1902) (ID:C1902) | [jrm](https://oraec.github.io/corpus/29840.html) | [jrm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=646&db=1) |
| [ⲙⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C1903) (ID:C1903) | [bn](https://oraec.github.io/corpus/55500.html) | [bn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1705&db=1) |
| [ⲙⲁⲉⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C1904) (ID:C1904) | [mn.w](https://oraec.github.io/corpus/70420.html) | [mn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2420&db=1) |
| [ⲙⲟⲩⲛ](https://coptic-dictionary.org/entry.cgi?tla=C1913) (ID:C1913) | [mn](https://oraec.github.io/corpus/69590.html) | [mn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2422&db=1) |
| [ⲙⲏⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1921) (ID:C1921) | [m-mn.t](https://oraec.github.io/corpus/64850.html) | [n-mney](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2428&db=1) |
| [ⲙⲓⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1922) (ID:C1922) | [mn.t](https://oraec.github.io/corpus/69760.html) | [mn.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2439&db=1) |
| [ⲙⲁⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1929) (ID:C1929) | [mnj.w](https://oraec.github.io/corpus/70310.html) | [mny](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2425&db=1) |
| [ⲙⲟⲟⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1931) (ID:C1931) | [mjni̯](https://oraec.github.io/corpus/854513.html) | [mn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-5140&db=1) |
| [ⲙⲟⲟⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1934) (ID:C1934) | [mnꜥ.t](https://oraec.github.io/corpus/70360.html) | [mn-jry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2437&db=1) |
| [ⲙⲛⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1936) (ID:C1936) | [mj-nꜣ](https://oraec.github.io/corpus/68390.html) |  |
| [ⲙⲛⲏ](https://coptic-dictionary.org/entry.cgi?tla=C1941) (ID:C1941) | [mj-nꜣ](https://oraec.github.io/corpus/68390.html) | [r-bw-nꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3368&db=1) |
| [ⲙⲟⲩⲛⲕ](https://coptic-dictionary.org/entry.cgi?tla=C1945) (ID:C1945) | [mnq](https://oraec.github.io/corpus/71400.html) | [mnqe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2478&db=1) |
| [ⲙⲟⲩⲛⲕ](https://coptic-dictionary.org/entry.cgi?tla=C1950) (ID:C1950) | [mnq](https://oraec.github.io/corpus/71400.html) | [mnqe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2478&db=1) |
| [ⲙⲟⲛⲙⲉⲛ](https://coptic-dictionary.org/entry.cgi?tla=C1956) (ID:C1956) | [mnmn](https://oraec.github.io/corpus/70710.html) | [mnmn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2464&db=1) |
| [ⲙⲛⲧ-](https://coptic-dictionary.org/entry.cgi?tla=C1961) (ID:C1961) | [mdw.t](https://oraec.github.io/corpus/78030.html) | [md.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2753&db=1) |
| [ⲙⲛⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1962) (ID:C1962) | [mnḏ](https://oraec.github.io/corpus/71720.html) | [mnt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4210&db=1) |
| [ⲙⲛⲟⲩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1964) (ID:C1964) | [wnw.tj](https://oraec.github.io/corpus/46450.html) | [mnṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2487&db=1) |
| [ⲙⲛⲟⲩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C1965) (ID:C1965) | [wnw.tj](https://oraec.github.io/corpus/46450.html) | [mnṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2487&db=1) |
| [ⲙⲛⲧⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C1967) (ID:C1967) | [mtr.w](https://oraec.github.io/corpus/77760.html) | [mtre](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2803&db=1) |
| [ⲙⲡⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C1971) (ID:C1971) |  | [mbꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2412&db=1) |
| [ⲙⲡⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C1972) (ID:C1972) | [bn-pw](https://oraec.github.io/corpus/600469.html) | [bn-pw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-26&db=1) |
| [ⲙⲡⲟ](https://coptic-dictionary.org/entry.cgi?tla=C1974) (ID:C1974) | [jnbꜣ](https://oraec.github.io/corpus/27260.html) | [ꜣbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-222&db=1) |
| [ⲙⲡⲣ-](https://coptic-dictionary.org/entry.cgi?tla=C1979) (ID:C1979) | [m-jri̯](https://oraec.github.io/corpus/600050.html) | [m-jr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2233&db=1) |
| [ⲙⲡⲁⲧⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C1981) (ID:C1981) |  | [bw-jr-tw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1693&db=1) |
| [ⲙⲏⲣ](https://coptic-dictionary.org/entry.cgi?tla=C1990) (ID:C1990) | [mrw](https://oraec.github.io/corpus/72630.html) | [mr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2529&db=1) |
| [ⲙⲟⲩⲣ](https://coptic-dictionary.org/entry.cgi?tla=C1991) (ID:C1991) | [mr](https://oraec.github.io/corpus/71880.html) | [mre](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2492&db=1) |
| [ⲙⲟⲩⲣ](https://coptic-dictionary.org/entry.cgi?tla=C1992) (ID:C1992) | [mr](https://oraec.github.io/corpus/855067.html) | [mlꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2566&db=1) |
| [ⲙⲁⲣ](https://coptic-dictionary.org/entry.cgi?tla=C1999) (ID:C1999) | [mr.w](https://oraec.github.io/corpus/72120.html) | [mre.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-47&db=1) |
| [ⲙⲁⲓⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2000) (ID:C2000) | [mr.t](https://oraec.github.io/corpus/72010.html) | [mre.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-47&db=1) |
| [ⲙⲉⲣⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C2005) (ID:C2005) |  | [bw-jr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1692&db=1) |
| [ⲙⲉⲉⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2006) (ID:C2006) | [mtr.t](https://oraec.github.io/corpus/77710.html) | [mtre.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2796&db=1) |
| [ⲙⲣⲱ](https://coptic-dictionary.org/entry.cgi?tla=C2008) (ID:C2008) | [mr.yt](https://oraec.github.io/corpus/72540.html) | [mr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2529&db=1) |
| [ⲙⲣⲱⲙ](https://coptic-dictionary.org/entry.cgi?tla=C2010) (ID:C2010) | [wrm](https://oraec.github.io/corpus/47820.html) |  |
| [ⲙⲣⲓⲥ](https://coptic-dictionary.org/entry.cgi?tla=C2014) (ID:C2014) | [mrsw](https://oraec.github.io/corpus/72940.html) | [mysl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2351&db=1) |
| [ⲙⲟⲣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2015) (ID:C2015) | [mrt](https://oraec.github.io/corpus/73040.html) | [mrṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2561&db=1) |
| [ⲙⲣⲟϣ](https://coptic-dictionary.org/entry.cgi?tla=C2017) (ID:C2017) |  | [mlš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2581&db=1) |
| [ⲙⲏⲣϣ](https://coptic-dictionary.org/entry.cgi?tla=C2018) (ID:C2018) |  | [mlš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2581&db=1) |
| [ⲙⲉⲣⲉϩ](https://coptic-dictionary.org/entry.cgi?tla=C2025) (ID:C2025) | [mrḥ](https://oraec.github.io/corpus/72830.html) |  |
| [ⲙⲣⲏϩ](https://coptic-dictionary.org/entry.cgi?tla=C2027) (ID:C2027) | [mrḥ](https://oraec.github.io/corpus/72830.html) |  |
| [ⲙⲣⲱϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2028) (ID:C2028) | [mtrḫ.t](https://oraec.github.io/corpus/77800.html) | [mrḫ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2556&db=1) |
| [ⲙⲓⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2035) (ID:C2035) | [msi̯](https://oraec.github.io/corpus/74950.html) | [ms](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2672&db=1) |
| [ⲙⲏⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2044) (ID:C2044) | [msw.t](https://oraec.github.io/corpus/75070.html) | [ms.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2679&db=1) |
| [ⲙⲁⲥ](https://coptic-dictionary.org/entry.cgi?tla=C2045) (ID:C2045) | [ms](https://oraec.github.io/corpus/74750.html) | [ms](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2674&db=1) |
| [ⲙⲁⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2046) (ID:C2046) | [ms](https://oraec.github.io/corpus/74770.html) | [ms](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2675&db=1) |
| [ⲙⲏⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2047) (ID:C2047) | [ms](https://oraec.github.io/corpus/74780.html) | [ms.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2677&db=1) |
| [ⲙⲉⲥⲓⲱ](https://coptic-dictionary.org/entry.cgi?tla=C2053) (ID:C2053) |  | [ms-ꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2676&db=1) |
| [ⲙⲟⲩⲥⲕ](https://coptic-dictionary.org/entry.cgi?tla=C2055) (ID:C2055) | [msq](https://oraec.github.io/corpus/75870.html) |  |
| [ⲙⲟⲥⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2057) (ID:C2057) | [msḏi̯](https://oraec.github.io/corpus/76210.html) | [msdy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2693&db=1) |
| [ⲙⲉⲥⲑⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2064) (ID:C2064) | [mstj](https://oraec.github.io/corpus/76010.html) |  |
| [ⲙⲥⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C2067) (ID:C2067) | [mzḥ](https://oraec.github.io/corpus/75590.html) | [msḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2689&db=1) |
| [ⲙⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2069) (ID:C2069) | [mḏ](https://oraec.github.io/corpus/78340.html) |  |
| [ⲙⲏⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2070) (ID:C2070) | [mḏ](https://oraec.github.io/corpus/78340.html) |  |
| [ⲙⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2071) (ID:C2071) | [mꜣt.t](https://oraec.github.io/corpus/67500.html) |  |
| [ⲙⲟⲉⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2072) (ID:C2072) | [mṯn](https://oraec.github.io/corpus/77960.html) | [myt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2354&db=1) |
| [ⲙⲟⲩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2082) (ID:C2082) | [mt](https://oraec.github.io/corpus/77310.html) | [mt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2742&db=1) |
| [ⲙⲁⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2084) (ID:C2084) | [mtj](https://oraec.github.io/corpus/400854.html) | [mtry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2797&db=1) |
| [ⲙⲁⲧⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2093) (ID:C2093) | [mḏꜣ.y](https://oraec.github.io/corpus/854516.html) | [Mdy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2767&db=1) |
| [ⲙⲏⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2096) (ID:C2096) |  | [mtre.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2800&db=1) |
| [ⲙⲟⲩⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2101) (ID:C2101) | [mdwi̯](https://oraec.github.io/corpus/78140.html) | [md](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2765&db=1) |
| [ⲙⲧⲟ](https://coptic-dictionary.org/entry.cgi?tla=C2116) (ID:C2116) |  | [mtr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4524&db=1) |
| [ⲙⲧⲱ](https://coptic-dictionary.org/entry.cgi?tla=C2117) (ID:C2117) | [mḏw.t](https://oraec.github.io/corpus/78610.html) | [mt.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4171&db=1) |
| [ⲙⲧⲱ](https://coptic-dictionary.org/entry.cgi?tla=C2118) (ID:C2118) | [mtr](https://oraec.github.io/corpus/77690.html) | [mtry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2801&db=1) |
| [ⲙⲧⲟⲛ](https://coptic-dictionary.org/entry.cgi?tla=C2122) (ID:C2122) | [mdn](https://oraec.github.io/corpus/78220.html) | [mtn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2792&db=1) |
| [ⲙⲧⲟⲛ](https://coptic-dictionary.org/entry.cgi?tla=C2123) (ID:C2123) | [mdn](https://oraec.github.io/corpus/78220.html) | [mtn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2792&db=1) |
| [ⲙⲧⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2146) (ID:C2146) | [mdw](https://oraec.github.io/corpus/78150.html) | [md.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2753&db=1) |
| [ⲙⲁⲧⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2150) (ID:C2150) | [mtw.t](https://oraec.github.io/corpus/854515.html) | [mtw.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3035&db=1) |
| [ⲙⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2155) (ID:C2155) | [jm](https://oraec.github.io/corpus/24640.html) | [n.jm=w](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2942&db=1) |
| [ⲙⲙⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2156) (ID:C2156) | [jm](https://oraec.github.io/corpus/24640.html) | [n.jm=w](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2942&db=1) |
| [ⲉⲧⲙⲙⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2157) (ID:C2157) | [n.tj-jm](https://oraec.github.io/corpus/89900.html) |  |
| [ⲙⲁⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2160) (ID:C2160) | [mw.t](https://oraec.github.io/corpus/69040.html) | [mw.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2380&db=1) |
| [ⲙⲁⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2161) (ID:C2161) | [mw.t](https://oraec.github.io/corpus/69040.html) | [mw.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2380&db=1) |
| [ⲙⲁⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2164) (ID:C2164) | [mw.t](https://oraec.github.io/corpus/69040.html) | [mw.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2380&db=1) |
| [ⲙⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2165) (ID:C2165) | [mw](https://oraec.github.io/corpus/69000.html) | [mw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2378&db=1) |
| [ⲙⲁⲩⲁⲁ⸗](https://coptic-dictionary.org/entry.cgi?tla=C2176) (ID:C2176) |  | [wꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1258&db=1) |
| [ⲙⲉⲉⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2178) (ID:C2178) | [mꜣwṯ](https://oraec.github.io/corpus/67590.html) | [mwy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2393&db=1) |
| [ⲙⲁⲟⲩⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2191) (ID:C2191) | [mjz.t](https://oraec.github.io/corpus/68520.html) | [mws](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2405&db=1) |
| [ⲙⲟⲩⲟⲩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2192) (ID:C2192) | [mwt](https://oraec.github.io/corpus/69300.html) | [mwt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2408&db=1) |
| [ⲙⲁϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2195) (ID:C2195) | [mḫꜣ.t](https://oraec.github.io/corpus/74300.html) | [mḫy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2646&db=1) |
| [ⲙⲁϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2196) (ID:C2196) | [mḫꜣ.t](https://oraec.github.io/corpus/74300.html) | [mḫy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2646&db=1) |
| [ⲉⲙⲁϣⲟ](https://coptic-dictionary.org/entry.cgi?tla=C2198) (ID:C2198) | [m-šs](https://oraec.github.io/corpus/600392.html) | [m-šs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2254&db=1) |
| [ⲙⲙⲁϣⲱ](https://coptic-dictionary.org/entry.cgi?tla=C2199) (ID:C2199) | [m-šs](https://oraec.github.io/corpus/600392.html) | [m-šs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2254&db=1) |
| [ⲙⲏⲏϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2203) (ID:C2203) | [mšꜥ](https://oraec.github.io/corpus/76300.html) | [mšꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2702&db=1) |
| [ⲙⲓϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2207) (ID:C2207) |  | [mh̭y](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2644&db=1) |
| [ⲙⲓϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2208) (ID:C2208) |  | [mh̭y](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2644&db=1) |
| [ⲙⲟⲟϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2219) (ID:C2219) | [mšꜥ](https://oraec.github.io/corpus/76330.html) | [mšꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2701&db=1) |
| [ⲙⲉϣⲡⲉⲗⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2257) (ID:C2257) |  | [mšprṱ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2703&db=1) |
| [ⲙⲁϣⲣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2260) (ID:C2260) |  | [mšḥṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2707&db=1) |
| [ⲙⲁϣⲣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2261) (ID:C2261) |  | [mšḥṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2707&db=1) |
| [ⲙⲟⲩϣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2262) (ID:C2262) |  | [mšdey](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2710&db=1) |
| [ⲙⲏϣⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2270) (ID:C2270) | [mšd.t](https://oraec.github.io/corpus/76620.html) | [mšty](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2711&db=1) |
| [ⲙϣⲓϣ](https://coptic-dictionary.org/entry.cgi?tla=C2273) (ID:C2273) |  | [mšyḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2699&db=1) |
| [ⲙⲁϧⲟⲩⲗ](https://coptic-dictionary.org/entry.cgi?tla=C2280) (ID:C2280) | [mnḫ](https://oraec.github.io/corpus/71060.html) | [myẖl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2348&db=1) |
| [ⲙⲙⲁϩ-](https://coptic-dictionary.org/entry.cgi?tla=C2281) (ID:C2281) | [m-bꜣḥ](https://oraec.github.io/corpus/64750.html) | [m-bꜣḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2238&db=1) |
| [ⲙⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C2282) (ID:C2282) | [mḥ](https://oraec.github.io/corpus/73400.html) | [mḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4833&db=1) |
| [ⲙⲁϩⲟⲩⲁⲗ](https://coptic-dictionary.org/entry.cgi?tla=C2283) (ID:C2283) | [mḥwn](https://oraec.github.io/corpus/74010.html) | [mḥwl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2635&db=1) |
| [ⲙⲟⲉⲓϩ](https://coptic-dictionary.org/entry.cgi?tla=C2284) (ID:C2284) | [mḥ.t](https://oraec.github.io/corpus/73530.html) | [myḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2343&db=1) |
| [ⲙⲟⲩϩ](https://coptic-dictionary.org/entry.cgi?tla=C2285) (ID:C2285) | [mḥ](https://oraec.github.io/corpus/854514.html) | [mḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2596&db=1) |
| [ⲙⲉϩ-](https://coptic-dictionary.org/entry.cgi?tla=C2296) (ID:C2296) |  | [mḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2597&db=1) |
| [ⲙⲟⲩϩ](https://coptic-dictionary.org/entry.cgi?tla=C2297) (ID:C2297) | [mꜣẖ](https://oraec.github.io/corpus/67280.html) | [mẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2659&db=1) |
| [ⲙⲟⲩϩ](https://coptic-dictionary.org/entry.cgi?tla=C2299) (ID:C2299) |  | [mẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2661&db=1) |
| [ⲙⲁϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2301) (ID:C2301) | [mḥ](https://oraec.github.io/corpus/73330.html) | [mḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2599&db=1) |
| [ⲙⲁϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2302) (ID:C2302) | [mḥꜥ.w](https://oraec.github.io/corpus/450266.html) | [mḥe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2602&db=1) |
| [ⲙⲏϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2305) (ID:C2305) | [mḥ.t](https://oraec.github.io/corpus/73500.html) | [mḥy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2626&db=1) |
| [ⲙⲟⲉⲓϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2307) (ID:C2307) |  | [myhꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2341&db=1) |
| [ⲙⲟⲉⲓϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2308) (ID:C2308) |  | [myhꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2341&db=1) |
| [ⲙϩⲏ](https://coptic-dictionary.org/entry.cgi?tla=C2310) (ID:C2310) | [mḥ.yt](https://oraec.github.io/corpus/73860.html) | [mḥy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2619&db=1) |
| [ⲙⲉϩⲏⲗ](https://coptic-dictionary.org/entry.cgi?tla=C2311) (ID:C2311) |  | [mhl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2591&db=1) |
| [ⲙⲉϩⲙⲟⲩϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2312) (ID:C2312) | [mḫmḫw.t](https://oraec.github.io/corpus/74370.html) |  |
| [ⲙⲟⲩϧⲣⲏⲣ](https://coptic-dictionary.org/entry.cgi?tla=C2315) (ID:C2315) |  | [mẖrr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2665&db=1) |
| [ⲙⲁϩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2316) (ID:C2316) | [mẖt.w](https://oraec.github.io/corpus/74690.html) | [mẖṱe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2671&db=1) |
| [ⲙϩⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2323) (ID:C2323) | [mḥ.tj](https://oraec.github.io/corpus/73561.html) | [mḥṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2640&db=1) |
| [ⲙϩⲁⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2325) (ID:C2325) | [mꜥḥꜥ.t](https://oraec.github.io/corpus/68920.html) | [mhwe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2585&db=1) |
| [ⲙϩⲁⲟⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2326) (ID:C2326) | [mhw.t](https://oraec.github.io/corpus/73130.html) | [mhwꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2586&db=1) |
| [ⲙⲁⲁϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2328) (ID:C2328) | [msḏr](https://oraec.github.io/corpus/76230.html) | [msḏr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2696&db=1) |
| [ⲙⲁⲁϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2330) (ID:C2330) |  | [mḏꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2842&db=1) |
| [ⲙⲁϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2331) (ID:C2331) | [mḏꜣ.t](https://oraec.github.io/corpus/78480.html) | [mḏy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2847&db=1) |
| [ⲙⲁϫⲁⲕⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C2333) (ID:C2333) |  | [mḏqn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2862&db=1) |
| [ⲙϫⲱⲗ](https://coptic-dictionary.org/entry.cgi?tla=C2335) (ID:C2335) |  | [mḏl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2858&db=1) |
| [ⲙⲟϫϩ](https://coptic-dictionary.org/entry.cgi?tla=C2339) (ID:C2339) | [mḏḥ](https://oraec.github.io/corpus/78670.html) | [mḏẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2860&db=1) |
| [ⲙⲟⲩϫϭ](https://coptic-dictionary.org/entry.cgi?tla=C2342) (ID:C2342) |  | [mṯk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2837&db=1) |
| [ⲙⲉϭⲧⲱⲗ](https://coptic-dictionary.org/entry.cgi?tla=C2346) (ID:C2346) | [mktr](https://oraec.github.io/corpus/77140.html) | [mkṱl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2733&db=1) |
| [ⲛ](https://coptic-dictionary.org/entry.cgi?tla=C11279) (ID:C11279) | [=n](https://oraec.github.io/corpus/10070.html) | [=n](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2866&db=1) |
| [ⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C2348) (ID:C2348) | [n.j](https://oraec.github.io/corpus/850787.html) | [n](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2869&db=1) |
| [ⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C2349) (ID:C2349) | [m](https://oraec.github.io/corpus/64360.html) | [n](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2871&db=1) |
| [ⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C2350) (ID:C2350) | [n](https://oraec.github.io/corpus/78870.html) | [n](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2870&db=1) |
| [ⲛ- (ⲁⲛ)](https://coptic-dictionary.org/entry.cgi?tla=C2351) (ID:C2351) | [bn](https://oraec.github.io/corpus/55500.html) | [bn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1705&db=1) |
| [ⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C2352) (ID:C2352) | [nꜣ](https://oraec.github.io/corpus/851623.html) | [nꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2952&db=1) |
| [ⲛⲁ-](https://coptic-dictionary.org/entry.cgi?tla=C2354) (ID:C2354) | [nꜣ-n](https://oraec.github.io/corpus/79580.html) | [nꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-73&db=1) |
| [ⲛⲁ](https://coptic-dictionary.org/entry.cgi?tla=C2356) (ID:C2356) | [nꜥi̯](https://oraec.github.io/corpus/80340.html) | [nꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3069&db=1) |
| [ⲛⲁ](https://coptic-dictionary.org/entry.cgi?tla=C2371) (ID:C2371) | [nꜥi̯](https://oraec.github.io/corpus/854518.html) | [nꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3070&db=1) |
| [ⲛⲁ-](https://coptic-dictionary.org/entry.cgi?tla=C2381) (ID:C2381) | [nꜥi̯](https://oraec.github.io/corpus/854518.html) | [nꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2962&db=1) |
| [ⲛⲁⲉⲓⲱ](https://coptic-dictionary.org/entry.cgi?tla=C2383) (ID:C2383) | [nꜥy.t](https://oraec.github.io/corpus/80450.html) | [nꜥy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3071&db=1) |
| [ⲛⲉ⸗](https://coptic-dictionary.org/entry.cgi?tla=C2384) (ID:C2384) | [nꜣy=](https://oraec.github.io/corpus/550008.html) | [nꜣy=](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3021&db=1) |
| [ⲛⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C2386) (ID:C2386) |  | [wn-nꜣ.w](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1368&db=1) |
| [ⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2387) (ID:C2387) |  | [nꜣ.w](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3009&db=1) |
| [ⲛⲉⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2389) (ID:C2389) | [nr](https://oraec.github.io/corpus/85100.html) | [nꜣy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3020&db=1) |
| [ⲛⲏ](https://coptic-dictionary.org/entry.cgi?tla=C2393) (ID:C2393) | [nꜣ](https://oraec.github.io/corpus/851623.html) | [nꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3017&db=1) |
| [ⲛⲟⲩ⸗](https://coptic-dictionary.org/entry.cgi?tla=C2394) (ID:C2394) |  | [nꜣy=](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3022&db=1) |
| [ⲛⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2395) (ID:C2395) | [nꜥi̯](https://oraec.github.io/corpus/854518.html) | [nꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3070&db=1) |
| [ⲛⲏⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2397) (ID:C2397) |  | [jn-jw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=547&db=1) |
| [ⲛⲏⲃ](https://coptic-dictionary.org/entry.cgi?tla=C2417) (ID:C2417) | [nb](https://oraec.github.io/corpus/81650.html) | [nb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3104&db=1) |
| [ⲛⲏⲃ](https://coptic-dictionary.org/entry.cgi?tla=C2418) (ID:C2418) | [nb](https://oraec.github.io/corpus/81650.html) | [nb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3104&db=1) |
| [ⲛⲟⲩⲃ](https://coptic-dictionary.org/entry.cgi?tla=C2427) (ID:C2427) | [nbw](https://oraec.github.io/corpus/81680.html) | [nb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3106&db=1) |
| [ⲛⲏⲏⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2429) (ID:C2429) | [nbi̯](https://oraec.github.io/corpus/82530.html) | [nby](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3125&db=1) |
| [ⲛⲟⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2432) (ID:C2432) |  | [nby](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3122&db=1) |
| [ⲛⲟⲩⲃⲥ](https://coptic-dictionary.org/entry.cgi?tla=C2441) (ID:C2441) | [nbs](https://oraec.github.io/corpus/82810.html) | [nbs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3136&db=1) |
| [ⲛⲟⲩⲃⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2442) (ID:C2442) | [nbd](https://oraec.github.io/corpus/82850.html) | [nbt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3138&db=1) |
| [ⲛⲏⲃⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2443) (ID:C2443) | [nbd](https://oraec.github.io/corpus/82870.html) | [nbd.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3142&db=1) |
| [ⲛⲉⲃⲑⲱ](https://coptic-dictionary.org/entry.cgi?tla=C2444) (ID:C2444) | [Nb.t-ḥw.t](https://oraec.github.io/corpus/82260.html) | [Nb.t-ḥ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3117&db=1) |
| [ⲛⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2445) (ID:C2445) | [nꜣj](https://oraec.github.io/corpus/851663.html) | [nꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3017&db=1) |
| [ⲛⲟⲉⲓⲕ](https://coptic-dictionary.org/entry.cgi?tla=C2446) (ID:C2446) | [nk.w](https://oraec.github.io/corpus/89240.html) | [nk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3286&db=1) |
| [ⲛⲁⲁⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2450) (ID:C2450) | [nqꜥ.wt](https://oraec.github.io/corpus/854710.html) |  |
| [ⲛⲕⲁ](https://coptic-dictionary.org/entry.cgi?tla=C2452) (ID:C2452) | [nkt](https://oraec.github.io/corpus/600036.html) | [nkt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3290&db=1) |
| [ⲛⲟⲩⲕⲉⲣ](https://coptic-dictionary.org/entry.cgi?tla=C2456) (ID:C2456) |  | [nqr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3284&db=1) |
| [ⲛⲕⲟⲧⲕ](https://coptic-dictionary.org/entry.cgi?tla=C2458) (ID:C2458) | [nqdd](https://oraec.github.io/corpus/89190.html) | [jn-qdy.ṱ.k](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=558&db=1) |
| [ⲛⲓⲙ](https://coptic-dictionary.org/entry.cgi?tla=C2473) (ID:C2473) | [jn-m](https://oraec.github.io/corpus/27410.html) | [nme](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3164&db=1) |
| [ⲛⲓⲙ](https://coptic-dictionary.org/entry.cgi?tla=C2474) (ID:C2474) | [nb](https://oraec.github.io/corpus/81660.html) | [nb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3105&db=1) |
| [ⲛⲓⲙ](https://coptic-dictionary.org/entry.cgi?tla=C2475) (ID:C2475) | [nb](https://oraec.github.io/corpus/81660.html) | [nb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3105&db=1) |
| [ⲛⲉⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2477) (ID:C2477) |  | [nm.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3173&db=1) |
| [ⲛⲟⲙⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2479) (ID:C2479) | [nmt.t](https://oraec.github.io/corpus/84510.html) | [nmt.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-2317&db=1) |
| [ⲛⲟⲉⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C2486) (ID:C2486) | [njnj](https://oraec.github.io/corpus/80170.html) | [nyn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3058&db=1) |
| [ⲛⲟⲩⲛ](https://coptic-dictionary.org/entry.cgi?tla=C2490) (ID:C2490) | [nw.w](https://oraec.github.io/corpus/500005.html) | [nwn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3095&db=1) |
| [ⲛⲏⲛⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2498) (ID:C2498) | [mn](https://oraec.github.io/corpus/69630.html) | [nny.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3198&db=1) |
| [ⲛⲏⲛⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2499) (ID:C2499) | [mn](https://oraec.github.io/corpus/69630.html) | [nny.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3198&db=1) |
| [ⲛⲟⲩⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2502) (ID:C2502) | [mny.t](https://oraec.github.io/corpus/70220.html) | [nn.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4361&db=1) |
| [ⲛⲟⲩⲛⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2503) (ID:C2503) | [mny.t](https://oraec.github.io/corpus/70220.html) | [nn.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4361&db=1) |
| [ⲛⲛⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C2504) (ID:C2504) |  | [bn-jw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1714&db=1) |
| [ⲛⲉⲛⲉⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2506) (ID:C2506) | [nnjb](https://oraec.github.io/corpus/84920.html) | [*nnyb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3894&db=1) |
| [ⲛⲁⲡⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2507) (ID:C2507) | [npn.t](https://oraec.github.io/corpus/83110.html) | [npny](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3149&db=1) |
| [ⲛⲁⲡⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2508) (ID:C2508) | [npr](https://oraec.github.io/corpus/83140.html) | [npy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3148&db=1) |
| [ⲛⲟⲩⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2510) (ID:C2510) | [nr.t](https://oraec.github.io/corpus/85040.html) | [nry.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3205&db=1) |
| [ⲛⲟⲩⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2511) (ID:C2511) | [nr.t](https://oraec.github.io/corpus/85040.html) | [nry.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3205&db=1) |
| [ⲛⲟⲩⲣⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2512) (ID:C2512) | [nr.t](https://oraec.github.io/corpus/85040.html) | [nry.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3205&db=1) |
| [ⲛⲟⲩⲣⲥ](https://coptic-dictionary.org/entry.cgi?tla=C2513) (ID:C2513) | [nsr](https://oraec.github.io/corpus/88270.html) |  |
| [ⲛⲏⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2519) (ID:C2519) | [ns.t](https://oraec.github.io/corpus/87870.html) | [nsy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3263&db=1) |
| [ⲛⲁⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2522) (ID:C2522) | [nḏ](https://oraec.github.io/corpus/90960.html) | [nt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3299&db=1) |
| [ⲛⲟⲩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2523) (ID:C2523) | [nḏ](https://oraec.github.io/corpus/90880.html) | [nt.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3298&db=1) |
| [ⲛⲟⲉⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2527) (ID:C2527) | [nḏ](https://oraec.github.io/corpus/90900.html) | [nyt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3063&db=1) |
| [ⲛⲟⲩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2529) (ID:C2529) |  | [nwṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-807&db=1) |
| [ⲛⲧⲁ-](https://coptic-dictionary.org/entry.cgi?tla=C2530) (ID:C2530) |  | [nty-jw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-358&db=1) |
| [ⲛⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2531) (ID:C2531) | [mtw=](https://oraec.github.io/corpus/600030.html) | [mtw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2779&db=1) |
| [ⲛⲧⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C2532) (ID:C2532) | [m-dj](https://oraec.github.io/corpus/600056.html) | [mtw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2781&db=1) |
| [ⲛⲧⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C2533) (ID:C2533) | [m-dj](https://oraec.github.io/corpus/860665.html) | [nty](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3302&db=1) |
| [ⲛⲧⲟ](https://coptic-dictionary.org/entry.cgi?tla=C2534) (ID:C2534) | [jntṯ](https://oraec.github.io/corpus/90160.html) |  |
| [ⲛⲟⲩⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2535) (ID:C2535) | [nṯr](https://oraec.github.io/corpus/90260.html) | [nṯr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3318&db=1) |
| [ⲛⲧⲱⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2536) (ID:C2536) | [nṯr.t](https://oraec.github.io/corpus/90280.html) | [nṯr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3320&db=1) |
| [ⲛⲉⲧⲟ](https://coptic-dictionary.org/entry.cgi?tla=C2537) (ID:C2537) | [nṯr-ꜥꜣ](https://oraec.github.io/corpus/90360.html) | [nṯr-ꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4991&db=1) |
| [ⲛⲟⲩⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2538) (ID:C2538) | [nṯr.j](https://oraec.github.io/corpus/400281.html) | [nṯrey](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3323&db=1) |
| [ⲛⲧⲟⲕ](https://coptic-dictionary.org/entry.cgi?tla=C2556) (ID:C2556) | [jntk](https://oraec.github.io/corpus/90120.html) |  |
| [ⲛⲟⲩⲧⲙ](https://coptic-dictionary.org/entry.cgi?tla=C2557) (ID:C2557) | [nḏm](https://oraec.github.io/corpus/500020.html) | [nḏm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3314&db=1) |
| [ⲛⲟⲩⲧⲉⲙ](https://coptic-dictionary.org/entry.cgi?tla=C2558) (ID:C2558) | [nḏm](https://oraec.github.io/corpus/91410.html) | [nḏm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3297&db=1) |
| [ⲛⲧⲉⲣⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C2561) (ID:C2561) |  | [n-ḏr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2938&db=1) |
| [ⲛⲧⲟⲥ](https://coptic-dictionary.org/entry.cgi?tla=C2562) (ID:C2562) | [jnts](https://oraec.github.io/corpus/90080.html) |  |
| [ⲛⲧⲟⲥ](https://coptic-dictionary.org/entry.cgi?tla=C2563) (ID:C2563) | [jnts](https://oraec.github.io/corpus/90080.html) |  |
| [ⲛⲧⲟⲥ](https://coptic-dictionary.org/entry.cgi?tla=C2564) (ID:C2564) | [jnts](https://oraec.github.io/corpus/90080.html) |  |
| [ⲛⲧⲱⲧⲛ](https://coptic-dictionary.org/entry.cgi?tla=C2565) (ID:C2565) | [jntṯn](https://oraec.github.io/corpus/90170.html) |  |
| [ⲛⲧⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2566) (ID:C2566) | [ntw](https://oraec.github.io/corpus/89980.html) |  |
| [ⲛⲧⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2567) (ID:C2567) | [ntw](https://oraec.github.io/corpus/89980.html) |  |
| [ⲛⲧⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2568) (ID:C2568) | [ntw](https://oraec.github.io/corpus/89980.html) |  |
| [ⲛⲧⲟⲟⲩⲛ](https://coptic-dictionary.org/entry.cgi?tla=C2569) (ID:C2569) | [m-dwn](https://oraec.github.io/corpus/66000.html) |  |
| [ⲛⲟⲩⲧϥ](https://coptic-dictionary.org/entry.cgi?tla=C2570) (ID:C2570) | [nft](https://oraec.github.io/corpus/83950.html) | [ntf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3313&db=1) |
| [ⲛⲧⲟϥ](https://coptic-dictionary.org/entry.cgi?tla=C2572) (ID:C2572) | [jntf](https://oraec.github.io/corpus/90020.html) |  |
| [ⲛⲧⲟϥ](https://coptic-dictionary.org/entry.cgi?tla=C2573) (ID:C2573) | [jntf](https://oraec.github.io/corpus/90020.html) |  |
| [ⲛⲧⲟϥ](https://coptic-dictionary.org/entry.cgi?tla=C2574) (ID:C2574) | [jntf](https://oraec.github.io/corpus/90020.html) |  |
| [ⲛⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2578) (ID:C2578) | [nwꜣ](https://oraec.github.io/corpus/80800.html) | [nwe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3081&db=1) |
| [ⲛⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C2589) (ID:C2589) | [nw](https://oraec.github.io/corpus/80840.html) | [nw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3085&db=1) |
| [ⲛⲁⲩⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2593) (ID:C2593) | [njw.y](https://oraec.github.io/corpus/80060.html) | [nw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3089&db=1) |
| [ⲛⲱⲟⲩϯ](https://coptic-dictionary.org/entry.cgi?tla=C2595) (ID:C2595) | [nwd.t](https://oraec.github.io/corpus/81570.html) |  |
| [ⲛⲟⲩϩ](https://coptic-dictionary.org/entry.cgi?tla=C2596) (ID:C2596) | [nwḥ](https://oraec.github.io/corpus/81410.html) |  |
| [ⲛⲟⲉⲓϣ](https://coptic-dictionary.org/entry.cgi?tla=C2598) (ID:C2598) | [nnšm](https://oraec.github.io/corpus/85010.html) | [nyš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3062&db=1) |
| [ⲛⲟⲟϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2602) (ID:C2602) | [nꜥš](https://oraec.github.io/corpus/80650.html) | [nꜥš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1101&db=1) |
| [ⲛⲟⲩϣⲡ](https://coptic-dictionary.org/entry.cgi?tla=C2603) (ID:C2603) | [nšp](https://oraec.github.io/corpus/88620.html) |  |
| [ⲛⲟϣⲣ](https://coptic-dictionary.org/entry.cgi?tla=C2606) (ID:C2606) |  | [nšr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3279&db=1) |
| [ⲛⲟⲩϣⲥ](https://coptic-dictionary.org/entry.cgi?tla=C2607) (ID:C2607) | [snḫt](https://oraec.github.io/corpus/138010.html) |  |
| [ⲛϣⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2610) (ID:C2610) | [nšw.t](https://oraec.github.io/corpus/88400.html) | [nšy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3275&db=1) |
| [ⲛⲟⲩϣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2611) (ID:C2611) | [nḫt](https://oraec.github.io/corpus/87560.html) | [nḫṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3252&db=1) |
| [ⲛϣⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2613) (ID:C2613) | [nḫt](https://oraec.github.io/corpus/87560.html) | [nḫṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3252&db=1) |
| [ⲛⲁϣⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2619) (ID:C2619) | [nḫt.w](https://oraec.github.io/corpus/87620.html) | [nḫṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1448&db=1) |
| [ⲛⲁϣⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2620) (ID:C2620) | [nḫt.t](https://oraec.github.io/corpus/87600.html) | [nḫṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1448&db=1) |
| [ⲛⲉϣⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2622) (ID:C2622) | [nḫt](https://oraec.github.io/corpus/87580.html) |  |
| [ⲛⲉⲉϥ](https://coptic-dictionary.org/entry.cgi?tla=C2623) (ID:C2623) | [nf.wj](https://oraec.github.io/corpus/83420.html) | [nf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3155&db=1) |
| [ⲛⲓϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2627) (ID:C2627) | [nfi̯](https://oraec.github.io/corpus/83380.html) | [nfy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-240&db=1) |
| [ⲛⲓϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2628) (ID:C2628) |  | [nef](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4801&db=1) |
| [*ⲛⲟⲩϥⲣ](https://coptic-dictionary.org/entry.cgi?tla=C2632) (ID:C2632) | [nfr](https://oraec.github.io/corpus/854519.html) | [nfr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3275&db=1) |
| [ⲛⲟϥⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2633) (ID:C2633) | [nfr.t](https://oraec.github.io/corpus/83680.html) | [nfr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-191&db=1) |
| [ⲛⲟⲩϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2637) (ID:C2637) | [nfr](https://oraec.github.io/corpus/550034.html) | [nfr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3156&db=1) |
| [ⲛⲉϩ](https://coptic-dictionary.org/entry.cgi?tla=C2640) (ID:C2640) | [nḥḥ](https://oraec.github.io/corpus/86600.html) | [nḥḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3238&db=1) |
| [ⲛⲟϩ](https://coptic-dictionary.org/entry.cgi?tla=C2643) (ID:C2643) | [jnḥ](https://oraec.github.io/corpus/27700.html) | [jnḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=585&db=1) |
| [ⲛⲟⲩϩ](https://coptic-dictionary.org/entry.cgi?tla=C2644) (ID:C2644) | [nwḥ](https://oraec.github.io/corpus/81400.html) | [nwḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3100&db=1) |
| [ⲛⲟϩⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2650) (ID:C2650) |  | [nwḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3100&db=1) |
| [ⲛⲟⲩϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2651) (ID:C2651) | [nh](https://oraec.github.io/corpus/85210.html) |  |
| [ⲛⲟⲩϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2654) (ID:C2654) | [nh.t](https://oraec.github.io/corpus/85290.html) | [nhy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3215&db=1) |
| [ⲛⲟⲩϩⲃ](https://coptic-dictionary.org/entry.cgi?tla=C2655) (ID:C2655) | [nḥb](https://oraec.github.io/corpus/86130.html) | [nḥbe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3233&db=1) |
| [ⲛⲁϩⲃ](https://coptic-dictionary.org/entry.cgi?tla=C2656) (ID:C2656) | [nḥb](https://oraec.github.io/corpus/86150.html) | [nḥbe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-2221&db=1) |
| [ⲛⲁϩⲃ](https://coptic-dictionary.org/entry.cgi?tla=C2658) (ID:C2658) | [nḥb.t](https://oraec.github.io/corpus/86210.html) | [nḥbe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-2221&db=1) |
| [ⲛⲟⲩϩⲃ](https://coptic-dictionary.org/entry.cgi?tla=C2659) (ID:C2659) | [nhp](https://oraec.github.io/corpus/854520.html) |  |
| [ⲛⲟⲩϩⲙ](https://coptic-dictionary.org/entry.cgi?tla=C2662) (ID:C2662) | [nḥm](https://oraec.github.io/corpus/86430.html) | [nḥm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3235&db=1) |
| [ⲛⲉϩⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2667) (ID:C2667) | [nhp](https://oraec.github.io/corpus/85490.html) | [nhpy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3220&db=1) |
| [ⲛϩⲟⲩⲣ](https://coptic-dictionary.org/entry.cgi?tla=C2671) (ID:C2671) | [nhr](https://oraec.github.io/corpus/85710.html) | [nhwr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-2099&db=1) |
| [ⲛⲉϩⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2674) (ID:C2674) | [nhzi̯](https://oraec.github.io/corpus/85790.html) | [nhsꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3225&db=1) |
| [ⲛⲁϩⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2676) (ID:C2676) | [nḥti̯](https://oraec.github.io/corpus/86680.html) | [nḥṱy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3241&db=1) |
| [ⲛⲟⲩϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2691) (ID:C2691) | [nḏri̯](https://oraec.github.io/corpus/91670.html) |  |
| [ⲛⲟⲩϫⲕ](https://coptic-dictionary.org/entry.cgi?tla=C2706) (ID:C2706) |  | [nḏḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3334&db=1) |
| [ⲛⲁϫϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2711) (ID:C2711) | [nḥḏ.t](https://oraec.github.io/corpus/86750.html) | [nḏḥy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3333&db=1) |
| [ⲛⲟϭ](https://coptic-dictionary.org/entry.cgi?tla=C2712) (ID:C2712) | [qni̯](https://oraec.github.io/corpus/854565.html) | [qny](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3257&db=1) |
| [ⲛϭⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2723) (ID:C2723) |  | [n-ge](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2932&db=1) |
| [ⲛⲟϭⲛⲉϭ](https://coptic-dictionary.org/entry.cgi?tla=C2724) (ID:C2724) | [ngg](https://oraec.github.io/corpus/89720.html) | [ngnge](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3294&db=1) |
| [ⲟ](https://coptic-dictionary.org/entry.cgi?tla=C2734) (ID:C2734) | [ꜥꜣ](https://oraec.github.io/corpus/450158.html) | [ꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=825&db=1) |
| [ⲟⲃ](https://coptic-dictionary.org/entry.cgi?tla=C2735) (ID:C2735) | [ꜥb.w](https://oraec.github.io/corpus/36300.html) |  |
| [ⲟⲃⲛ](https://coptic-dictionary.org/entry.cgi?tla=C2738) (ID:C2738) | [jbn.w](https://oraec.github.io/corpus/23770.html) | [ꜣbn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=80&db=1) |
| [ⲟⲃϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2739) (ID:C2739) | [jbḥ](https://oraec.github.io/corpus/23830.html) | [ꜣbḥy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=83&db=1) |
| [ⲟⲉⲓⲕ](https://coptic-dictionary.org/entry.cgi?tla=C2740) (ID:C2740) | [ꜥq.w](https://oraec.github.io/corpus/41470.html) | [ꜥq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1123&db=1) |
| [ⲥⲁ ⲛⲱⲓⲕ](https://coptic-dictionary.org/entry.cgi?tla=C2742) (ID:C2742) |  | [s-n-ꜥq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-2539&db=1) |
| [ⲟⲉⲓⲕ](https://coptic-dictionary.org/entry.cgi?tla=C2743) (ID:C2743) |  | [ꜥkꜣr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1139&db=1) |
| [ⲟⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2744) (ID:C2744) | [jk](https://oraec.github.io/corpus/32440.html) | [ꜣqy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=233&db=1) |
| [ⲟⲉⲓⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2745) (ID:C2745) | [jjr](https://oraec.github.io/corpus/21420.html) | [ꜣywr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=15&db=1) |
| [ⲟⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2746) (ID:C2746) | [ꜥmꜥ.t](https://oraec.github.io/corpus/37740.html) | [ꜥmy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=967&db=1) |
| [ⲟⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2747) (ID:C2747) | [ꜥmꜥ.t](https://oraec.github.io/corpus/37740.html) | [ꜥmy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=967&db=1) |
| [ⲟⲉⲓⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2753) (ID:C2753) | [ḥꜣm.t](https://oraec.github.io/corpus/101440.html) | [ḥm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-475&db=1) |
| [ⲟⲛ](https://coptic-dictionary.org/entry.cgi?tla=C2754) (ID:C2754) | [ꜥn](https://oraec.github.io/corpus/38050.html) | [ꜥn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=973&db=1) |
| [ⲟⲉⲓⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2756) (ID:C2756) | [jp.t](https://oraec.github.io/corpus/24120.html) | [jpy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=465&db=1) |
| [ⲟⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2758) (ID:C2758) | [js](https://oraec.github.io/corpus/31250.html) | [ꜣsy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=212&db=1) |
| [ⲟⲥⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2761) (ID:C2761) | [jzr](https://oraec.github.io/corpus/31610.html) | [ꜣsr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=222&db=1) |
| [ⲟⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2763) (ID:C2763) | [jꜣd](https://oraec.github.io/corpus/21140.html) | [ꜣt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-317&db=1) |
| [ⲟⲟⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2764) (ID:C2764) | [jd.t](https://oraec.github.io/corpus/850291.html) | [ꜣty.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=264&db=1) |
| [ⲟⲟⲩϣ](https://coptic-dictionary.org/entry.cgi?tla=C2765) (ID:C2765) | [jwšš](https://oraec.github.io/corpus/23110.html) | [ꜥwš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4346&db=1) |
| [ⲟⲉⲓϣ](https://coptic-dictionary.org/entry.cgi?tla=C2766) (ID:C2766) | [ꜥš](https://oraec.github.io/corpus/40900.html) | [ꜥš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-5535&db=1) |
| [ⲟⲟϩ](https://coptic-dictionary.org/entry.cgi?tla=C2777) (ID:C2777) | [jꜥḥ](https://oraec.github.io/corpus/21810.html) | [jꜥḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=353&db=1) |
| [ⲟϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2778) (ID:C2778) | [jh.w](https://oraec.github.io/corpus/30210.html) | [jhy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=662&db=1) |
| [ⲟϫⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2779) (ID:C2779) | [ꜥḏꜣ](https://oraec.github.io/corpus/42100.html) | [ꜥḏ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1162&db=1) |
| [ⲟϫⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2780) (ID:C2780) | [ꜥḏꜣ](https://oraec.github.io/corpus/42120.html) | [ꜥḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3636&db=1) |
| [ⲡ-](https://coptic-dictionary.org/entry.cgi?tla=C2783) (ID:C2783) | [pꜣ](https://oraec.github.io/corpus/851446.html) | [pꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1839&db=1) |
| [ⲡⲁ-](https://coptic-dictionary.org/entry.cgi?tla=C2785) (ID:C2785) | [pꜣ-n](https://oraec.github.io/corpus/550051.html) | [pa](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1931&db=1) |
| [ⲡⲉ⸗](https://coptic-dictionary.org/entry.cgi?tla=C2786) (ID:C2786) | [pꜣy=](https://oraec.github.io/corpus/550021.html) | [pꜣy=](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1925&db=1) |
| [ⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2788) (ID:C2788) | [pꜣj](https://oraec.github.io/corpus/851661.html) | [pꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1921&db=1) |
| [ⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2790) (ID:C2790) | [p.t](https://oraec.github.io/corpus/58710.html) | [p.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1838&db=1) |
| [ⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2791) (ID:C2791) | [pꜣi̯](https://oraec.github.io/corpus/58780.html) | [pꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1922&db=1) |
| [ⲡⲏⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2792) (ID:C2792) | [pꜣi̯](https://oraec.github.io/corpus/58780.html) | [pꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1922&db=1) |
| [ⲡⲏ](https://coptic-dictionary.org/entry.cgi?tla=C2794) (ID:C2794) | [pꜣj](https://oraec.github.io/corpus/851661.html) | [pꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1920&db=1) |
| [ⲡⲏ](https://coptic-dictionary.org/entry.cgi?tla=C2795) (ID:C2795) | [pꜥ.t](https://oraec.github.io/corpus/59610.html) |  |
| [ϯⲡⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2797) (ID:C2797) |  | [typy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7097&db=1) |
| [ⲡⲱ⸗](https://coptic-dictionary.org/entry.cgi?tla=C2798) (ID:C2798) |  | [pꜣy=](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1926&db=1) |
| [ⲡⲓⲁ](https://coptic-dictionary.org/entry.cgi?tla=C2799) (ID:C2799) | [pꜣi̯](https://oraec.github.io/corpus/58780.html) | [pꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1922&db=1) |
| [ⲡⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2800) (ID:C2800) | [pꜣj](https://oraec.github.io/corpus/851661.html) | [pꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1920&db=1) |
| [ⲡⲏⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2801) (ID:C2801) | [pr.yt](https://oraec.github.io/corpus/61010.html) |  |
| [ⲡⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2802) (ID:C2802) | [pj](https://oraec.github.io/corpus/58650.html) | [py](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1941&db=1) |
| [ⲡⲁⲓⲁⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2803) (ID:C2803) |  | [Pyt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1954&db=1) |
| [ⲡⲁⲕ](https://coptic-dictionary.org/entry.cgi?tla=C2808) (ID:C2808) | [pgꜣ](https://oraec.github.io/corpus/854511.html) |  |
| [ⲡⲁⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2809) (ID:C2809) | [pꜣqi̯](https://oraec.github.io/corpus/59300.html) |  |
| [ⲡⲱⲗϭ](https://coptic-dictionary.org/entry.cgi?tla=C2820) (ID:C2820) |  | [plk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2112&db=1) |
| [ⲡⲟⲙⲡⲉⲙ](https://coptic-dictionary.org/entry.cgi?tla=C2831) (ID:C2831) | [bnbn](https://oraec.github.io/corpus/55770.html) |  |
| [ⲡⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C2832) (ID:C2832) | [pn.w](https://oraec.github.io/corpus/60020.html) | [pn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1978&db=1) |
| [ⲡⲱⲛ](https://coptic-dictionary.org/entry.cgi?tla=C2835) (ID:C2835) | [pnn](https://oraec.github.io/corpus/60030.html) | [pne](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1977&db=1) |
| [ⲡⲱⲱⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2837) (ID:C2837) | [pnꜥ](https://oraec.github.io/corpus/59960.html) | [pnꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1981&db=1) |
| [ⲡⲱⲛⲕ](https://coptic-dictionary.org/entry.cgi?tla=C2847) (ID:C2847) | [pnq](https://oraec.github.io/corpus/60130.html) | [pnq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1983&db=1) |
| [ⲫⲱⲛⲕ](https://coptic-dictionary.org/entry.cgi?tla=C2852) (ID:C2852) | [pnq](https://oraec.github.io/corpus/60130.html) | [pnq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1983&db=1) |
| [ⲡⲛⲛⲏ](https://coptic-dictionary.org/entry.cgi?tla=C2856) (ID:C2856) | [pnꜥ.yt](https://oraec.github.io/corpus/59990.html) | [pnꜥꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-230&db=1) |
| [ⲡⲁⲡⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2858) (ID:C2858) | [npꜣpꜣ](https://oraec.github.io/corpus/83010.html) | [ppy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1971&db=1) |
| [ⲡⲱⲱⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2859) (ID:C2859) | [pjpj](https://oraec.github.io/corpus/59540.html) | [ppy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1972&db=1) |
| [ⲡⲣⲱ](https://coptic-dictionary.org/entry.cgi?tla=C2862) (ID:C2862) | [pr.t](https://oraec.github.io/corpus/60300.html) | [pr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2078&db=1) |
| [ⲡⲉⲣ-](https://coptic-dictionary.org/entry.cgi?tla=C2863) (ID:C2863) | [pr](https://oraec.github.io/corpus/60220.html) | [pr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1985&db=1) |
| [ⲡⲏⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2868) (ID:C2868) | [pꜣꜥ.t](https://oraec.github.io/corpus/401147.html) | [pꜥry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1939&db=1) |
| [ⲡⲉⲓⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2869) (ID:C2869) | [pri̯](https://oraec.github.io/corpus/60920.html) | [pr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2083&db=1) |
| [ⲡⲱⲱⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2874) (ID:C2874) | [ptr](https://oraec.github.io/corpus/62900.html) | [pry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2084&db=1) |
| [ⲡⲟⲣⲕ](https://coptic-dictionary.org/entry.cgi?tla=C2876) (ID:C2876) |  | [prk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2099&db=1) |
| [ⲡⲱⲣⲕ](https://coptic-dictionary.org/entry.cgi?tla=C2880) (ID:C2880) |  | [prq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2098&db=1) |
| [ⲡⲉⲣⲛⲟⲩϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2888) (ID:C2888) |  | [pr-nfr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2042&db=1) |
| [ⲡⲉⲣⲓⲡⲉⲣⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C2890) (ID:C2890) |  | [pr-pr-ꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2028&db=1) |
| [ⲡⲏⲣϣ](https://coptic-dictionary.org/entry.cgi?tla=C2894) (ID:C2894) | [prš](https://oraec.github.io/corpus/61260.html) | [prš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2096&db=1) |
| [ⲡⲱⲣϣ](https://coptic-dictionary.org/entry.cgi?tla=C2895) (ID:C2895) | [prḫ](https://oraec.github.io/corpus/61240.html) | [prḫe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2091&db=1) |
| [ⲡⲱⲣϫ](https://coptic-dictionary.org/entry.cgi?tla=C2903) (ID:C2903) |  | [prḏe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2105&db=1) |
| [ⲡⲓⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2912) (ID:C2912) | [psi̯](https://oraec.github.io/corpus/62180.html) | [psy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2142&db=1) |
| [ⲯⲓⲥ](https://coptic-dictionary.org/entry.cgi?tla=C2919) (ID:C2919) | [psḏ](https://oraec.github.io/corpus/62450.html) |  |
| [ⲯⲓⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2920) (ID:C2920) | [psḏ](https://oraec.github.io/corpus/62450.html) |  |
| [ⲡⲁⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2922) (ID:C2922) | [pꜣḏ](https://oraec.github.io/corpus/59460.html) | [pd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2179&db=1) |
| [ⲡⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2925) (ID:C2925) | [pꜣd](https://oraec.github.io/corpus/59440.html) | [pd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2178&db=1) |
| [ⲡⲓⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2933) (ID:C2933) | [pḏ.t](https://oraec.github.io/corpus/63270.html) | [pty.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2181&db=1) |
| [ⲡⲟⲧⲡⲉⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2936) (ID:C2936) | [ptpt](https://oraec.github.io/corpus/62890.html) |  |
| [ⲡⲱⲧⲥ](https://coptic-dictionary.org/entry.cgi?tla=C2937) (ID:C2937) | [pds](https://oraec.github.io/corpus/63120.html) |  |
| [ⲡⲁⲧⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2939) (ID:C2939) | [pds](https://oraec.github.io/corpus/63110.html) | [pds](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2187&db=1) |
| [ⲡⲱⲧϩ](https://coptic-dictionary.org/entry.cgi?tla=C2940) (ID:C2940) |  | [ptḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2186&db=1) |
| [ⲡⲧⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C2942) (ID:C2942) | [Ptḥ](https://oraec.github.io/corpus/62980.html) | [Ptḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2185&db=1) |
| [ⲡⲁⲩⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2944) (ID:C2944) | [pr.w](https://oraec.github.io/corpus/61140.html) | [pr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1990&db=1) |
| [ⲡⲁϣ](https://coptic-dictionary.org/entry.cgi?tla=C2946) (ID:C2946) | [pḫꜣ](https://oraec.github.io/corpus/61780.html) | [pḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2131&db=1) |
| [ⲡⲱϣ](https://coptic-dictionary.org/entry.cgi?tla=C2949) (ID:C2949) | [psš](https://oraec.github.io/corpus/62280.html) | [pše](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2150&db=1) |
| [ⲡⲁϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2956) (ID:C2956) | [psš.t](https://oraec.github.io/corpus/62290.html) | [pše.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2152&db=1) |
| [ⲡⲱϣⲛ](https://coptic-dictionary.org/entry.cgi?tla=C2958) (ID:C2958) | [pšn](https://oraec.github.io/corpus/62610.html) | [pšn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2155&db=1) |
| [ⲡⲱϣⲥ](https://coptic-dictionary.org/entry.cgi?tla=C2966) (ID:C2966) | [pzḫ](https://oraec.github.io/corpus/62240.html) |  |
| [ⲡⲱϩ](https://coptic-dictionary.org/entry.cgi?tla=C2973) (ID:C2973) | [pḫꜣ](https://oraec.github.io/corpus/61730.html) | [pẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2136&db=1) |
| [ⲡⲱϩ](https://coptic-dictionary.org/entry.cgi?tla=C2979) (ID:C2979) | [pḥ](https://oraec.github.io/corpus/61370.html) | [pḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2120&db=1) |
| [ⲡⲱϩⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2983) (ID:C2983) | [pẖr](https://oraec.github.io/corpus/61900.html) | [pẖr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2138&db=1) |
| [ⲡⲁϩⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2985) (ID:C2985) | [pẖr.t](https://oraec.github.io/corpus/61950.html) | [pẖreꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2139&db=1) |
| [ⲡⲁϩⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C2986) (ID:C2986) | [pẖr.t](https://oraec.github.io/corpus/61950.html) | [pẖreꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2139&db=1) |
| [ⲡⲱϩⲥ](https://coptic-dictionary.org/entry.cgi?tla=C2995) (ID:C2995) | [pzḥ](https://oraec.github.io/corpus/62220.html) | [pḥs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2127&db=1) |
| [ⲡⲱϩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C2997) (ID:C2997) | [pꜣḫd](https://oraec.github.io/corpus/59230.html) | [pẖṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2141&db=1) |
| [ⲡⲁϩⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3004) (ID:C3004) | [pḥ.tj](https://oraec.github.io/corpus/61400.html) | [pḥṱ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2124&db=1) |
| [ⲡⲁϩⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3005) (ID:C3005) | [pḥ.wj](https://oraec.github.io/corpus/61490.html) | [pḥw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2126&db=1) |
| [ⲡⲁϩⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3006) (ID:C3006) | [pḥ.wj](https://oraec.github.io/corpus/61490.html) | [pḥw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2126&db=1) |
| [ⲡⲟϫ](https://coptic-dictionary.org/entry.cgi?tla=C3016) (ID:C3016) |  | [pḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2191&db=1) |
| [ⲡⲱϫϭ](https://coptic-dictionary.org/entry.cgi?tla=C3019) (ID:C3019) |  | [pḏḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2192&db=1) |
| [ⲡⲱϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3023) (ID:C3023) | [pgꜣ](https://oraec.github.io/corpus/62730.html) | [pky](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2166&db=1) |
| [ⲡⲟϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3024) (ID:C3024) |  | [pk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2162&db=1) |
| [ⲡⲱϭⲥ](https://coptic-dictionary.org/entry.cgi?tla=C3026) (ID:C3026) | [psg](https://oraec.github.io/corpus/62340.html) |  |
| [ⲣⲁ](https://coptic-dictionary.org/entry.cgi?tla=C3029) (ID:C3029) | [rʾ-ꜥ](https://oraec.github.io/corpus/600214.html) | [rꜥ-](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3438&db=1) |
| [ⲣⲁ-](https://coptic-dictionary.org/entry.cgi?tla=C3030) (ID:C3030) | [rʾ-ꜥ](https://oraec.github.io/corpus/600214.html) | [rꜥ-](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3438&db=1) |
| [ⲣⲏ](https://coptic-dictionary.org/entry.cgi?tla=C3034) (ID:C3034) | [rꜥw](https://oraec.github.io/corpus/93290.html) | [rꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3436&db=1) |
| [ⲣⲏ](https://coptic-dictionary.org/entry.cgi?tla=C3035) (ID:C3035) | [rꜥw](https://oraec.github.io/corpus/93290.html) | [rꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3436&db=1) |
| [ⲣⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3037) (ID:C3037) | [rj.t](https://oraec.github.io/corpus/93230.html) | [ry.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3423&db=1) |
| [ⲣⲟ](https://coptic-dictionary.org/entry.cgi?tla=C3038) (ID:C3038) | [rʾ](https://oraec.github.io/corpus/92560.html) | [rꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3408&db=1) |
| [ⲣⲁ-](https://coptic-dictionary.org/entry.cgi?tla=C3049) (ID:C3049) | [rʾ](https://oraec.github.io/corpus/92630.html) | [rꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3411&db=1) |
| [ϩⲁⲣⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C3052) (ID:C3052) |  | [ẖr-rꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-2506&db=1) |
| [ϩⲓⲣⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C3053) (ID:C3053) |  | [ḥr-rꜣ-n](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4185&db=1) |
| [ⲣⲟ](https://coptic-dictionary.org/entry.cgi?tla=C3055) (ID:C3055) | [rʾ](https://oraec.github.io/corpus/92640.html) | [rꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3412&db=1) |
| [ⲣⲱ](https://coptic-dictionary.org/entry.cgi?tla=C3056) (ID:C3056) | [m-rʾ-ꜥ](https://oraec.github.io/corpus/64970.html) |  |
| [ⲣⲟⲉⲓⲥ](https://coptic-dictionary.org/entry.cgi?tla=C3058) (ID:C3058) | [rs](https://oraec.github.io/corpus/95940.html) | [rsy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3561&db=1) |
| [ⲣⲓⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3066) (ID:C3066) | [rqi̯](https://oraec.github.io/corpus/96290.html) | [lgy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3710&db=1) |
| [ⲣⲱⲕϩ](https://coptic-dictionary.org/entry.cgi?tla=C3080) (ID:C3080) | [rkḥ](https://oraec.github.io/corpus/96440.html) | [rqh](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3591&db=1) |
| [ⲣⲁⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3086) (ID:C3086) | [rm](https://oraec.github.io/corpus/94160.html) | [rm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3482&db=1) |
| [ⲣⲁⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3087) (ID:C3087) | [rm](https://oraec.github.io/corpus/94160.html) | [rm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3482&db=1) |
| [ⲣⲓⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3088) (ID:C3088) | [rmi̯](https://oraec.github.io/corpus/94180.html) | [rmy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3484&db=1) |
| [ⲣⲙⲉⲓⲏ](https://coptic-dictionary.org/entry.cgi?tla=C3090) (ID:C3090) | [rm.yt](https://oraec.github.io/corpus/94200.html) | [rmy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3485&db=1) |
| [ⲣⲱⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3092) (ID:C3092) | [rmṯ](https://oraec.github.io/corpus/94530.html) | [rmṯ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3491&db=1) |
| [ⲣⲱⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3093) (ID:C3093) | [rmṯ](https://oraec.github.io/corpus/94530.html) | [rmṯ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3491&db=1) |
| [ⲣⲱⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3094) (ID:C3094) | [rmṯ](https://oraec.github.io/corpus/94530.html) | [rmṯ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3491&db=1) |
| [ⲣⲱⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3095) (ID:C3095) | [rmṯ](https://oraec.github.io/corpus/94530.html) | [rmṯ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3491&db=1) |
| [ⲣⲙ-](https://coptic-dictionary.org/entry.cgi?tla=C3101) (ID:C3101) | [rmṯ](https://oraec.github.io/corpus/94530.html) | [rmṯ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3491&db=1) |
| [ⲣⲙⲙⲁⲟ](https://coptic-dictionary.org/entry.cgi?tla=C3103) (ID:C3103) | [rmṯ-ꜥꜣ](https://oraec.github.io/corpus/94600.html) | [rmṯ-ꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3500&db=1) |
| [ⲣⲟⲙⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3109) (ID:C3109) | [rnp.t](https://oraec.github.io/corpus/94920.html) | [rnp.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3519&db=1) |
| [ⲣⲁⲙⲥ](https://coptic-dictionary.org/entry.cgi?tla=C3114) (ID:C3114) | [rms](https://oraec.github.io/corpus/855219.html) | [rms](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3490&db=1) |
| [ⲣⲙϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3115) (ID:C3115) | [nmḥ.w](https://oraec.github.io/corpus/84370.html) | [nmḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3181&db=1) |
| [ⲣⲙϩⲏ](https://coptic-dictionary.org/entry.cgi?tla=C3116) (ID:C3116) | [nmḥ.yt](https://oraec.github.io/corpus/84360.html) | [nmḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3181&db=1) |
| [ⲣⲁⲛ](https://coptic-dictionary.org/entry.cgi?tla=C3121) (ID:C3121) | [rn](https://oraec.github.io/corpus/94700.html) | [rn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3515&db=1) |
| [ⲣⲏⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3128) (ID:C3128) | [rn](https://oraec.github.io/corpus/94720.html) |  |
| [ⲣⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3129) (ID:C3129) | [rʾ-pr](https://oraec.github.io/corpus/92870.html) | [rpy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3474&db=1) |
| [*ⲣⲡⲱ](https://coptic-dictionary.org/entry.cgi?tla=C3130) (ID:C3130) | [rnp.wt](https://oraec.github.io/corpus/95030.html) | [rpy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3473&db=1) |
| [ⲣⲓⲣ](https://coptic-dictionary.org/entry.cgi?tla=C3132) (ID:C3132) | [rr.j](https://oraec.github.io/corpus/95350.html) | [ryr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-162&db=1) |
| [ⲣⲁⲁⲣ](https://coptic-dictionary.org/entry.cgi?tla=C3137) (ID:C3137) | [rr.j](https://oraec.github.io/corpus/95350.html) | [ryr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-162&db=1) |
| [ⲣⲣⲟ](https://coptic-dictionary.org/entry.cgi?tla=C3138) (ID:C3138) | [pr-ꜥꜣ](https://oraec.github.io/corpus/60430.html) | [pr-ꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2002&db=1) |
| [ⲣⲣⲱ](https://coptic-dictionary.org/entry.cgi?tla=C3139) (ID:C3139) |  | [pr-ꜥꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2003&db=1) |
| [ⲣⲣⲟ](https://coptic-dictionary.org/entry.cgi?tla=C3140) (ID:C3140) | [pr-ꜥꜣ](https://oraec.github.io/corpus/60430.html) | [pr-ꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2002&db=1) |
| [ⲣⲉⲣⲙⲏ](https://coptic-dictionary.org/entry.cgi?tla=C3144) (ID:C3144) | [rmny.t](https://oraec.github.io/corpus/94410.html) |  |
| [ⲣⲥⲱ](https://coptic-dictionary.org/entry.cgi?tla=C3145) (ID:C3145) |  | [rs.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3563&db=1) |
| [ⲣⲁⲥⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3146) (ID:C3146) | [rs.wt](https://oraec.github.io/corpus/96130.html) | [rsweꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3575&db=1) |
| [ⲣⲏⲥ](https://coptic-dictionary.org/entry.cgi?tla=C3150) (ID:C3150) | [rs.j](https://oraec.github.io/corpus/96011.html) | [rsy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3569&db=1) |
| [ⲣⲏⲥ](https://coptic-dictionary.org/entry.cgi?tla=C3151) (ID:C3151) | [rs.j](https://oraec.github.io/corpus/96010.html) | [rsy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3569&db=1) |
| [ⲣⲁⲥⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3155) (ID:C3155) |  | [rsṱy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3582&db=1) |
| [ⲣⲁⲧ⸗](https://coptic-dictionary.org/entry.cgi?tla=C3162) (ID:C3162) | [rd](https://oraec.github.io/corpus/96600.html) | [rd.wy.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3606&db=1) |
| [ⲕⲁⲣⲁⲧ⸗](https://coptic-dictionary.org/entry.cgi?tla=C3164) (ID:C3164) |  | [ḫꜣꜥ rd.wy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4396&db=1) |
| [ⲉⲣⲁⲧ⸗](https://coptic-dictionary.org/entry.cgi?tla=C3173) (ID:C3173) |  | [r-rd.wy.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3377&db=1) |
| [ϩⲓⲣⲁⲧ⸗](https://coptic-dictionary.org/entry.cgi?tla=C3175) (ID:C3175) |  | [ḥr-rd.wy.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4186&db=1) |
| [ⲣⲉⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3176) (ID:C3176) | [ḥr.j-tꜣ](https://oraec.github.io/corpus/108880.html) |  |
| [ⲣⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3177) (ID:C3177) | [rwḏ.w](https://oraec.github.io/corpus/93850.html) | [rd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3599&db=1) |
| [ⲣⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3178) (ID:C3178) | [rd](https://oraec.github.io/corpus/96610.html) | [rd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3601&db=1) |
| [ⲣⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3179) (ID:C3179) | [rd](https://oraec.github.io/corpus/96620.html) | [rd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-6631&db=1) |
| [-ⲣⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3180) (ID:C3180) | [rwḏ](https://oraec.github.io/corpus/400633.html) | [lwt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3656&db=1) |
| [ⲣⲁⲓⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3182) (ID:C3182) |  | [ryṱ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3433&db=1) |
| [ⲣⲏⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3185) (ID:C3185) | [rd.wj](https://oraec.github.io/corpus/96640.html) | [rd.wy.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3608&db=1) |
| [ⲣⲱⲧⲉⲃ](https://coptic-dictionary.org/entry.cgi?tla=C3194) (ID:C3194) | [ndb.wt](https://oraec.github.io/corpus/90810.html) |  |
| [ⲣⲧⲟⲃ](https://coptic-dictionary.org/entry.cgi?tla=C3195) (ID:C3195) |  | [rtb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3611&db=1) |
| [ⲣⲁⲩⲏ](https://coptic-dictionary.org/entry.cgi?tla=C3196) (ID:C3196) | [rʾ-wꜣ.t](https://oraec.github.io/corpus/92830.html) |  |
| [ⲣⲟⲟⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3201) (ID:C3201) | [ꜥr.t](https://oraec.github.io/corpus/39210.html) | [ꜣrwy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=140&db=1) |
| [ⲣⲟⲟⲩⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3203) (ID:C3203) | [rnn.t](https://oraec.github.io/corpus/95130.html) | [rn.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3517&db=1) |
| [ⲣⲟⲟⲩⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3204) (ID:C3204) | [rnn.t](https://oraec.github.io/corpus/95130.html) | [rn.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3517&db=1) |
| [ⲣⲁⲟⲩⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3206) (ID:C3206) | [rwḏ.t](https://oraec.github.io/corpus/93880.html) |  |
| [ⲣⲟⲟⲩϣ](https://coptic-dictionary.org/entry.cgi?tla=C3207) (ID:C3207) | [wršu̯](https://oraec.github.io/corpus/48130.html) | [rwš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3462&db=1) |
| [ⲣⲁϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3222) (ID:C3222) | [ršu̯](https://oraec.github.io/corpus/96210.html) | [ršy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3586&db=1) |
| [ⲣⲟⲩϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3235) (ID:C3235) | [rwhꜣ](https://oraec.github.io/corpus/93690.html) | [rhy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3531&db=1) |
| [ⲣⲱϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3239) (ID:C3239) | [rḫt](https://oraec.github.io/corpus/95890.html) | [rḫṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3557&db=1) |
| [ⲣⲁϩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3242) (ID:C3242) | [rḫt.j](https://oraec.github.io/corpus/95930.html) | [rḫṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3558&db=1) |
| [ⲣⲱϩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3245) (ID:C3245) | [rḫt](https://oraec.github.io/corpus/95890.html) |  |
| [ⲣⲁϩⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3254) (ID:C3254) | [rhd.t](https://oraec.github.io/corpus/95500.html) | [rht](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3538&db=1) |
| [ⲣⲁϩⲧⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3255) (ID:C3255) |  | [rḥṱw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3541&db=1) |
| [ⲣⲟϫⲣⲉϫ](https://coptic-dictionary.org/entry.cgi?tla=C3258) (ID:C3258) |  | [rqrq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3590&db=1) |
| [ⲥ](https://coptic-dictionary.org/entry.cgi?tla=C3262) (ID:C3262) | [=s](https://oraec.github.io/corpus/10090.html) | [=s](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4934&db=1) |
| [ⲥⲁ](https://coptic-dictionary.org/entry.cgi?tla=C3263) (ID:C3263) | [sꜣ](https://oraec.github.io/corpus/125670.html) | [sꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-332&db=1) |
| [ⲛⲥⲁ-](https://coptic-dictionary.org/entry.cgi?tla=C3268) (ID:C3268) | [m-sꜣ](https://oraec.github.io/corpus/851454.html) | [m-sꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2250&db=1) |
| [ⲙⲛⲛⲥⲁ-](https://coptic-dictionary.org/entry.cgi?tla=C3269) (ID:C3269) |  | [bn m-sꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1711&db=1) |
| [ⲥⲁ](https://coptic-dictionary.org/entry.cgi?tla=C3271) (ID:C3271) | [z.t](https://oraec.github.io/corpus/125040.html) | [s.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4940&db=1) |
| [ⲥⲁ](https://coptic-dictionary.org/entry.cgi?tla=C3272) (ID:C3272) | [z](https://oraec.github.io/corpus/125010.html) | [s](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4938&db=1) |
| [ⲥⲁ ⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C3273) (ID:C3273) |  | [s-n-](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4941&db=1) |
| [ⲥⲁ](https://coptic-dictionary.org/entry.cgi?tla=C3274) (ID:C3274) | [sꜥꜣi̯](https://oraec.github.io/corpus/128660.html) |  |
| [ⲥⲁ](https://coptic-dictionary.org/entry.cgi?tla=C3275) (ID:C3275) | [sꜥꜣi̯](https://oraec.github.io/corpus/128660.html) | [sꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4985&db=1) |
| [ⲥⲁⲉⲓⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3276) (ID:C3276) | [sꜥꜣi̯](https://oraec.github.io/corpus/128660.html) |  |
| [ⲥⲁⲉⲓⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3277) (ID:C3277) | [sꜥꜣi̯](https://oraec.github.io/corpus/128660.html) |  |
| [ⲥⲁⲉⲓⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3278) (ID:C3278) | [sꜥꜣi̯](https://oraec.github.io/corpus/128660.html) |  |
| [ⲥⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C3283) (ID:C3283) | [st](https://oraec.github.io/corpus/400960.html) | [st](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5705&db=1) |
| [ⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3284) (ID:C3284) | [st](https://oraec.github.io/corpus/400960.html) | [st](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5706&db=1) |
| [ⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3285) (ID:C3285) | [st](https://oraec.github.io/corpus/147350.html) | [st](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5702&db=1) |
| [ⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3286) (ID:C3286) | [s.t](https://oraec.github.io/corpus/854540.html) | [s.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4948&db=1) |
| [ⲥⲉⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3288) (ID:C3288) | [sꜣi̯](https://oraec.github.io/corpus/126200.html) | [sy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5017&db=1) |
| [ⲥⲟ](https://coptic-dictionary.org/entry.cgi?tla=C3295) (ID:C3295) | [zꜣ](https://oraec.github.io/corpus/125600.html) | [sꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4969&db=1) |
| [ⲥⲱ](https://coptic-dictionary.org/entry.cgi?tla=C3302) (ID:C3302) | [sw.t](https://oraec.github.io/corpus/129610.html) |  |
| [ⲥⲱ](https://coptic-dictionary.org/entry.cgi?tla=C3303) (ID:C3303) | [sw.t](https://oraec.github.io/corpus/129610.html) |  |
| [ⲥⲱ](https://coptic-dictionary.org/entry.cgi?tla=C3304) (ID:C3304) | [zwr](https://oraec.github.io/corpus/130360.html) | [swr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5132&db=1) |
| [ⲥⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3312) (ID:C3312) | [sbꜣ](https://oraec.github.io/corpus/131200.html) | [sbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5177&db=1) |
| [ⲥⲃⲟ](https://coptic-dictionary.org/entry.cgi?tla=C3313) (ID:C3313) | [sbꜣ](https://oraec.github.io/corpus/131210.html) | [sbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5183&db=1) |
| [ⲥⲃⲱ](https://coptic-dictionary.org/entry.cgi?tla=C3314) (ID:C3314) | [sbꜣ.yt](https://oraec.github.io/corpus/131390.html) | [sbꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5185&db=1) |
| [ⲥⲁⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3327) (ID:C3327) | [sbꜣ.w](https://oraec.github.io/corpus/131320.html) |  |
| [ⲥⲁⲃⲏ](https://coptic-dictionary.org/entry.cgi?tla=C3328) (ID:C3328) | [sbꜣ.w](https://oraec.github.io/corpus/131320.html) |  |
| [ⲥⲁⲃⲏ](https://coptic-dictionary.org/entry.cgi?tla=C3329) (ID:C3329) | [sbꜣ.w](https://oraec.github.io/corpus/131320.html) |  |
| [ⲥⲁⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3330) (ID:C3330) | [sbꜣ](https://oraec.github.io/corpus/856678.html) | [sbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-910&db=1) |
| [ⲥⲁⲃⲏ](https://coptic-dictionary.org/entry.cgi?tla=C3331) (ID:C3331) | [sbꜣ](https://oraec.github.io/corpus/856678.html) | [sbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-910&db=1) |
| [ⲥⲃⲟⲩⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3337) (ID:C3337) | [sbꜣ](https://oraec.github.io/corpus/131230.html) |  |
| [ⲥⲏⲃ](https://coptic-dictionary.org/entry.cgi?tla=C3339) (ID:C3339) | [sbj](https://oraec.github.io/corpus/131530.html) | [sbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5182&db=1) |
| [ⲥⲏⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3340) (ID:C3340) | [sb.t](https://oraec.github.io/corpus/131120.html) | [sby.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5194&db=1) |
| [ⲥⲓⲃ](https://coptic-dictionary.org/entry.cgi?tla=C3343) (ID:C3343) | [zb.t](https://oraec.github.io/corpus/131040.html) | [syb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5033&db=1) |
| [ⲥⲱⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3344) (ID:C3344) | [zbṯ](https://oraec.github.io/corpus/132270.html) | [sby](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5193&db=1) |
| [ⲥⲃⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3351) (ID:C3351) | [sꜥb](https://oraec.github.io/corpus/128750.html) |  |
| [ⲥⲃⲟⲕ](https://coptic-dictionary.org/entry.cgi?tla=C3357) (ID:C3357) |  | [sbq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-8051&db=1) |
| [ⲥⲃⲗⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3360) (ID:C3360) | [zbn](https://oraec.github.io/corpus/131760.html) |  |
| [ⲥⲉⲃⲉⲛ](https://coptic-dictionary.org/entry.cgi?tla=C3361) (ID:C3361) | [sbn](https://oraec.github.io/corpus/131770.html) | [sbnꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5197&db=1) |
| [ⲥⲟⲃⲛ](https://coptic-dictionary.org/entry.cgi?tla=C3363) (ID:C3363) | [sbnj](https://oraec.github.io/corpus/131850.html) |  |
| [ⲥⲓⲃⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3364) (ID:C3364) |  | [sbt.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5221&db=1) |
| [ⲥⲟⲃⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3365) (ID:C3365) | [sbtj](https://oraec.github.io/corpus/132260.html) | [sbt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5222&db=1) |
| [ⲥⲟⲃⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3366) (ID:C3366) | [spdd](https://oraec.github.io/corpus/133370.html) | [sbty](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5224&db=1) |
| [ⲥⲃϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3373) (ID:C3373) | [sbḫ.t](https://oraec.github.io/corpus/131980.html) | [sbšy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5209&db=1) |
| [ⲥⲃⲱϩ](https://coptic-dictionary.org/entry.cgi?tla=C3374) (ID:C3374) | [sbḥ](https://oraec.github.io/corpus/131900.html) | [sbḥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5205&db=1) |
| [ⲥⲉⲥⲃⲟϩ](https://coptic-dictionary.org/entry.cgi?tla=C3375) (ID:C3375) |  | [s.t-sbḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4960&db=1) |
| [ⲥⲉⲥⲃⲟϩ](https://coptic-dictionary.org/entry.cgi?tla=C3376) (ID:C3376) |  | [s.t-sbḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4960&db=1) |
| [ⲥⲉⲥⲃⲟϩ](https://coptic-dictionary.org/entry.cgi?tla=C3377) (ID:C3377) |  | [s.t-sbḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4960&db=1) |
| [ⲥⲱⲃϩ](https://coptic-dictionary.org/entry.cgi?tla=C3379) (ID:C3379) |  | [sbḥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5204&db=1) |
| [ⲥⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3380) (ID:C3380) | [sꜣ](https://oraec.github.io/corpus/125670.html) | [sꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-332&db=1) |
| [ⲥⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3381) (ID:C3381) | [zꜣw](https://oraec.github.io/corpus/126360.html) | [sy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5016&db=1) |
| [ⲥⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3382) (ID:C3382) | [zꜣw](https://oraec.github.io/corpus/126360.html) | [sy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5016&db=1) |
| [ⲥⲱⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3385) (ID:C3385) | [zbi̯](https://oraec.github.io/corpus/131460.html) |  |
| [ⲥⲁⲉⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C3387) (ID:C3387) | [zwn.w](https://oraec.github.io/corpus/855957.html) | [swnw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5130&db=1) |
| [ⲥⲁⲉⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C3388) (ID:C3388) | [zwn.w](https://oraec.github.io/corpus/855957.html) | [swnw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5130&db=1) |
| [ⲥⲓⲟⲩⲣ](https://coptic-dictionary.org/entry.cgi?tla=C3390) (ID:C3390) | [sr](https://oraec.github.io/corpus/138920.html) | [sre](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5378&db=1) |
| [ⲥⲟⲉⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3391) (ID:C3391) |  | [syt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5065&db=1) |
| [ⲥⲓⲟⲟⲩⲛ](https://coptic-dictionary.org/entry.cgi?tla=C3397) (ID:C3397) |  | [s.t-jn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4951&db=1) |
| [ⲥⲟⲉⲓϣ](https://coptic-dictionary.org/entry.cgi?tla=C3398) (ID:C3398) |  | [syḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5052&db=1) |
| [ⲥⲁⲕ](https://coptic-dictionary.org/entry.cgi?tla=C3403) (ID:C3403) |  | [sqꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5642&db=1) |
| [ⲥⲟⲕ](https://coptic-dictionary.org/entry.cgi?tla=C3407) (ID:C3407) | [sꜣq](https://oraec.github.io/corpus/127380.html) | [sꜥq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5099&db=1) |
| [ⲥⲱⲕ](https://coptic-dictionary.org/entry.cgi?tla=C3408) (ID:C3408) | [sꜣq](https://oraec.github.io/corpus/127330.html) | [sq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5632&db=1) |
| [ⲥⲓⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3423) (ID:C3423) | [ski̯](https://oraec.github.io/corpus/854552.html) | [sq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5634&db=1) |
| [ⲥⲁⲕⲃⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3428) (ID:C3428) | [sqbb](https://oraec.github.io/corpus/146060.html) |  |
| [ⲥⲕⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3429) (ID:C3429) | [skꜣ](https://oraec.github.io/corpus/146610.html) | [skꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5658&db=1) |
| [ⲥⲕⲓⲙ](https://coptic-dictionary.org/entry.cgi?tla=C3431) (ID:C3431) | [skm](https://oraec.github.io/corpus/146790.html) |  |
| [ⲥⲕⲉⲛϩⲟ](https://coptic-dictionary.org/entry.cgi?tla=C3440) (ID:C3440) |  | [sq-n-ḥr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5639&db=1) |
| [ⲥⲕⲁⲡ](https://coptic-dictionary.org/entry.cgi?tla=C3442) (ID:C3442) | [sqbb.wj](https://oraec.github.io/corpus/146080.html) |  |
| [ⲥⲕⲟⲣⲕⲣ](https://coptic-dictionary.org/entry.cgi?tla=C3443) (ID:C3443) | [sqrqr](https://oraec.github.io/corpus/146260.html) | [sqlql](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-2753&db=1) |
| [ⲥⲗⲏ](https://coptic-dictionary.org/entry.cgi?tla=C3453) (ID:C3453) |  | [slꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5425&db=1) |
| [ⲥⲟⲗ](https://coptic-dictionary.org/entry.cgi?tla=C3454) (ID:C3454) |  | [sl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5422&db=1) |
| [ⲥⲱⲗ](https://coptic-dictionary.org/entry.cgi?tla=C3455) (ID:C3455) | [sꜣr](https://oraec.github.io/corpus/126840.html) | [sr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5383&db=1) |
| [ⲥⲟⲗⲥⲉⲗ](https://coptic-dictionary.org/entry.cgi?tla=C3475) (ID:C3475) |  | [slsl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5433&db=1) |
| [ⲥⲱⲗϭ](https://coptic-dictionary.org/entry.cgi?tla=C3499) (ID:C3499) |  | [slk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5435&db=1) |
| [ⲥⲗⲟϭⲗϭ](https://coptic-dictionary.org/entry.cgi?tla=C3503) (ID:C3503) |  | [srkrk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5412&db=1) |
| [ⲥⲙⲏ](https://coptic-dictionary.org/entry.cgi?tla=C3509) (ID:C3509) | [smj](https://oraec.github.io/corpus/134830.html) | [smy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7796&db=1) |
| [ⲥⲙⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3519) (ID:C3519) | [smꜣꜥ](https://oraec.github.io/corpus/134640.html) | [smꜣꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5287&db=1) |
| [ⲥⲓⲙ](https://coptic-dictionary.org/entry.cgi?tla=C3525) (ID:C3525) | [sm.w](https://oraec.github.io/corpus/134140.html) | [sm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5275&db=1) |
| [ⲥⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3526) (ID:C3526) | [sm.w](https://oraec.github.io/corpus/134140.html) | [sm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5275&db=1) |
| [ⲥⲱⲱⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3529) (ID:C3529) | [snꜥꜥ](https://oraec.github.io/corpus/136700.html) |  |
| [ⲥⲙⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3531) (ID:C3531) | [smj](https://oraec.github.io/corpus/134820.html) | [smy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5288&db=1) |
| [ⲁⲛⲥⲙⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3534) (ID:C3534) |  | [ꜥn-smy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7838&db=1) |
| [ⲥⲙⲓⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3537) (ID:C3537) | [smn](https://oraec.github.io/corpus/851677.html) | [smn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5298&db=1) |
| [ⲥⲙⲟⲩⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3544) (ID:C3544) | [smn](https://oraec.github.io/corpus/135180.html) | [smn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5297&db=1) |
| [ⲥⲙⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3557) (ID:C3557) |  | [smte](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5318&db=1) |
| [ⲥⲙⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3558) (ID:C3558) |  | [smte](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5318&db=1) |
| [ⲥⲱⲙⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3564) (ID:C3564) |  | [sꜥmt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5085&db=1) |
| [ⲥⲙⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3566) (ID:C3566) | [smꜣ](https://oraec.github.io/corpus/134360.html) | [sme](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5280&db=1) |
| [ⲥⲙⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C3567) (ID:C3567) |  | [smḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5307&db=1) |
| [ⲥⲁⲙⲁϩⲏⲣ](https://coptic-dictionary.org/entry.cgi?tla=C3571) (ID:C3571) |  | [šmre](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6040&db=1) |
| [ⲥⲏⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3573) (ID:C3573) | [snṯ.y](https://oraec.github.io/corpus/138640.html) | [snꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3579&db=1) |
| [ⲥⲓⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3575) (ID:C3575) | [zni̯](https://oraec.github.io/corpus/854546.html) | [sny](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5336&db=1) |
| [ⲥⲟⲛ](https://coptic-dictionary.org/entry.cgi?tla=C3583) (ID:C3583) | [sn](https://oraec.github.io/corpus/136230.html) | [sn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5324&db=1) |
| [ⲥⲟⲛ](https://coptic-dictionary.org/entry.cgi?tla=C3584) (ID:C3584) | [sn](https://oraec.github.io/corpus/136230.html) | [sn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5324&db=1) |
| [ⲥⲱⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3587) (ID:C3587) | [sn.t](https://oraec.github.io/corpus/136260.html) | [sn.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5330&db=1) |
| [ⲥⲱⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3588) (ID:C3588) | [sn.t](https://oraec.github.io/corpus/136260.html) | [sn.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5330&db=1) |
| [ⲥⲛⲁⲉⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C3591) (ID:C3591) |  | [snyn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5339&db=1) |
| [ⲥⲛⲏⲓⲛⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3593) (ID:C3593) |  | [snyn.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5341&db=1) |
| [ⲥⲱⲛⲕ](https://coptic-dictionary.org/entry.cgi?tla=C3594) (ID:C3594) | [snq](https://oraec.github.io/corpus/138280.html) | [snqy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5359&db=1) |
| [ⲥⲁⲛⲛⲉϩ](https://coptic-dictionary.org/entry.cgi?tla=C3599) (ID:C3599) | [znḥm](https://oraec.github.io/corpus/137910.html) |  |
| [ⲥⲛⲥⲛ](https://coptic-dictionary.org/entry.cgi?tla=C3602) (ID:C3602) | [snsn](https://oraec.github.io/corpus/138130.html) | [snsn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5356&db=1) |
| [ⲥⲛⲁⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3603) (ID:C3603) | [snḏ](https://oraec.github.io/corpus/138730.html) | [snd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5361&db=1) |
| [ⲥⲁⲛⲟⲩⲑ](https://coptic-dictionary.org/entry.cgi?tla=C3604) (ID:C3604) | [snḏ.w](https://oraec.github.io/corpus/138790.html) |  |
| [ⲥⲟⲛⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3605) (ID:C3605) | [snṯr](https://oraec.github.io/corpus/138670.html) | [snṯr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5368&db=1) |
| [ⲥⲱⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3606) (ID:C3606) | [snṯi̯](https://oraec.github.io/corpus/138620.html) | [snṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3322&db=1) |
| [ⲥⲛⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3613) (ID:C3613) | [snṯ.t](https://oraec.github.io/corpus/138580.html) | [snty.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-468&db=1) |
| [ⲥⲱⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3614) (ID:C3614) | [snṯi̯](https://oraec.github.io/corpus/138620.html) | [snṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3322&db=1) |
| [ⲥⲛⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3616) (ID:C3616) | [sn.w](https://oraec.github.io/corpus/136210.html) |  |
| [ⲥⲛⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3618) (ID:C3618) | [sn.w](https://oraec.github.io/corpus/136210.html) |  |
| [ⲙⲉϩⲥⲛⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3627) (ID:C3627) |  | [mḥ-2](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2607&db=1) |
| [ⲥⲁⲁⲛϣ](https://coptic-dictionary.org/entry.cgi?tla=C3629) (ID:C3629) | [sꜥnḫ](https://oraec.github.io/corpus/128910.html) | [sꜥnḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5087&db=1) |
| [ⲥⲛⲟϥ](https://coptic-dictionary.org/entry.cgi?tla=C3637) (ID:C3637) | [znf](https://oraec.github.io/corpus/137250.html) | [snfe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5349&db=1) |
| [ⲥⲛⲟⲩϥ](https://coptic-dictionary.org/entry.cgi?tla=C3642) (ID:C3642) | [snf](https://oraec.github.io/corpus/137300.html) | [snfe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5350&db=1) |
| [ⲥⲱⲛϩ](https://coptic-dictionary.org/entry.cgi?tla=C3643) (ID:C3643) | [snḥ](https://oraec.github.io/corpus/137850.html) | [snḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5355&db=1) |
| [ⲥⲛⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C3647) (ID:C3647) | [snḥ](https://oraec.github.io/corpus/500330.html) |  |
| [ⲥⲓⲛⲁϩⲃⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3648) (ID:C3648) | [snw-p.t](https://oraec.github.io/corpus/137210.html) | [snw-p.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5344&db=1) |
| [ⲥⲡ-](https://coptic-dictionary.org/entry.cgi?tla=C3649) (ID:C3649) |  | [ḥꜣ.t-sp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3935&db=1) |
| [ⲥⲡ-](https://coptic-dictionary.org/entry.cgi?tla=C3650) (ID:C3650) |  | [ḥꜣ.t-sp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3935&db=1) |
| [ⲥⲉⲉⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3651) (ID:C3651) | [zpi̯](https://oraec.github.io/corpus/132710.html) | [spy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5247&db=1) |
| [ⲥⲏⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3653) (ID:C3653) | [zp.yt](https://oraec.github.io/corpus/132730.html) | [sp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-745&db=1) |
| [ⲥⲏⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3654) (ID:C3654) | [zp.yt](https://oraec.github.io/corpus/132730.html) | [sp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-745&db=1) |
| [ⲥⲟⲡ](https://coptic-dictionary.org/entry.cgi?tla=C3655) (ID:C3655) | [zp](https://oraec.github.io/corpus/854543.html) | [sp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5230&db=1) |
| [ⲉⲟⲩⲥⲟⲡ](https://coptic-dictionary.org/entry.cgi?tla=C3662) (ID:C3662) |  | [n-wꜥ-sp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-531&db=1) |
| [ⲥⲱⲡ](https://coptic-dictionary.org/entry.cgi?tla=C3669) (ID:C3669) |  | [spy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5232&db=1) |
| [ⲥⲱⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3671) (ID:C3671) | [sp.t](https://oraec.github.io/corpus/132440.html) | [spꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5252&db=1) |
| [ⲥⲡⲗⲏⲗⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C3674) (ID:C3674) |  | [splelyn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5255&db=1) |
| [ⲥⲡⲓⲣ](https://coptic-dictionary.org/entry.cgi?tla=C3675) (ID:C3675) | [spr](https://oraec.github.io/corpus/132820.html) | [spyr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5251&db=1) |
| [ⲥⲡⲟⲧⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3683) (ID:C3683) | [sp.t](https://oraec.github.io/corpus/132440.html) | [spt.w](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5259&db=1) |
| [ⲥⲣⲟ](https://coptic-dictionary.org/entry.cgi?tla=C3684) (ID:C3684) | [zr](https://oraec.github.io/corpus/138880.html) | [jsw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=700&db=1) |
| [ⲥⲓⲣ](https://coptic-dictionary.org/entry.cgi?tla=C3685) (ID:C3685) |  | [syr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5046&db=1) |
| [ⲥⲓⲣ](https://coptic-dictionary.org/entry.cgi?tla=C3687) (ID:C3687) | [sr](https://oraec.github.io/corpus/138980.html) |  |
| [ⲥⲓⲣ](https://coptic-dictionary.org/entry.cgi?tla=C3688) (ID:C3688) | [zr](https://oraec.github.io/corpus/854835.html) |  |
| [ⲥⲟⲩⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3690) (ID:C3690) | [sr.t](https://oraec.github.io/corpus/139070.html) | [sr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5390&db=1) |
| [ⲥⲱⲣ](https://coptic-dictionary.org/entry.cgi?tla=C3694) (ID:C3694) |  | [sr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5382&db=1) |
| [ⲥⲟⲣⲙ](https://coptic-dictionary.org/entry.cgi?tla=C3703) (ID:C3703) | [zrm.t](https://oraec.github.io/corpus/139490.html) |  |
| [ⲥⲱⲣⲙ](https://coptic-dictionary.org/entry.cgi?tla=C3704) (ID:C3704) | [zbn](https://oraec.github.io/corpus/131760.html) | [srm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5401&db=1) |
| [ⲥⲣⲟⲙⲣⲙ](https://coptic-dictionary.org/entry.cgi?tla=C3714) (ID:C3714) | [zbnbn](https://oraec.github.io/corpus/131840.html) |  |
| [ⲥⲁⲣⲡⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3721) (ID:C3721) | [srp.t](https://oraec.github.io/corpus/139370.html) | [srpt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5396&db=1) |
| [ⲥⲣⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3723) (ID:C3723) | [srd](https://oraec.github.io/corpus/139920.html) |  |
| [ⲥⲟⲣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3724) (ID:C3724) | [sꜥr.t](https://oraec.github.io/corpus/129060.html) | [sꜥrṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5089&db=1) |
| [ⲥⲟⲣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3725) (ID:C3725) | [sꜥr.t](https://oraec.github.io/corpus/129060.html) | [sꜥrṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5089&db=1) |
| [ⲥⲣϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3732) (ID:C3732) | [srf](https://oraec.github.io/corpus/139410.html) | [srfy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5397&db=1) |
| [ⲥⲁⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3749) (ID:C3749) | [sꜣsꜣ](https://oraec.github.io/corpus/127250.html) | [sꜥsy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5096&db=1) |
| [ⲥⲓⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3751) (ID:C3751) | [zz.w](https://oraec.github.io/corpus/143740.html) |  |
| [ⲥⲟⲥⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3752) (ID:C3752) |  | [sꜥsꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5097&db=1) |
| [ⲥⲟⲩⲥⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3753) (ID:C3753) |  | [ssw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5586&db=1) |
| [ⲥⲟⲩⲥⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3754) (ID:C3754) |  | [swsw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5152&db=1) |
| [ⲥⲱⲥ](https://coptic-dictionary.org/entry.cgi?tla=C3755) (ID:C3755) | [sꜣsꜣ](https://oraec.github.io/corpus/127250.html) |  |
| [ⲥⲧⲱ](https://coptic-dictionary.org/entry.cgi?tla=C3759) (ID:C3759) | [sp.t](https://oraec.github.io/corpus/132440.html) |  |
| [ⲥⲁⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3760) (ID:C3760) | [sd](https://oraec.github.io/corpus/149520.html) | [sd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5709&db=1) |
| [ⲥⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3761) (ID:C3761) | [sd](https://oraec.github.io/corpus/149520.html) | [sd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5709&db=1) |
| [ⲥⲁⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3762) (ID:C3762) | [sḏ.t](https://oraec.github.io/corpus/150140.html) | [sty.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5728&db=1) |
| [ⲥⲁⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3763) (ID:C3763) | [sdꜣ](https://oraec.github.io/corpus/149660.html) |  |
| [ⲥⲉⲧⲏ](https://coptic-dictionary.org/entry.cgi?tla=C3765) (ID:C3765) | [snṯ.t](https://oraec.github.io/corpus/138580.html) | [snty.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-468&db=1) |
| [ⲥⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3766) (ID:C3766) | [Stẖ](https://oraec.github.io/corpus/148520.html) | [Stḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5767&db=1) |
| [ⲥⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3767) (ID:C3767) | [zꜣ-tꜣ](https://oraec.github.io/corpus/126130.html) | [syt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5069&db=1) |
| [ⲥⲓⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3768) (ID:C3768) | [sti̯](https://oraec.github.io/corpus/854553.html) | [sty](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5725&db=1) |
| [ⲥⲟⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3775) (ID:C3775) | [st.w](https://oraec.github.io/corpus/147890.html) | [sty.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5727&db=1) |
| [ⲥⲟⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3776) (ID:C3776) | [st.w](https://oraec.github.io/corpus/147890.html) | [sty.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5727&db=1) |
| [ⲥⲓⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3781) (ID:C3781) |  | [stw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5730&db=1) |
| [ⲥⲟⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3782) (ID:C3782) |  | [sṱy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-510&db=1) |
| [ⲥⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3785) (ID:C3785) | [sṯꜣ.t](https://oraec.github.io/corpus/148840.html) | [sṯꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5716&db=1) |
| [ⲥⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3787) (ID:C3787) | [sṯꜣ](https://oraec.github.io/corpus/854555.html) | [sṯꜣ.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5720&db=1) |
| [ⲥⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3789) (ID:C3789) | [sṯꜣ](https://oraec.github.io/corpus/854555.html) | [sṯꜣ.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5720&db=1) |
| [ⲥⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3792) (ID:C3792) | [sṯꜣ](https://oraec.github.io/corpus/854555.html) | [sṯꜣ.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5720&db=1) |
| [ⲥⲁⲧⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3798) (ID:C3798) | [sdb](https://oraec.github.io/corpus/149770.html) |  |
| [ⲥⲧⲉⲃⲁⲉⲓϩ](https://coptic-dictionary.org/entry.cgi?tla=C3800) (ID:C3800) | [sdbḥ](https://oraec.github.io/corpus/149790.html) | [stbḥ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5733&db=1) |
| [ⲥⲟⲧⲃⲉϥ](https://coptic-dictionary.org/entry.cgi?tla=C3801) (ID:C3801) |  | [stbḥ=f](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5734&db=1) |
| [ⲥⲧⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3806) (ID:C3806) | [sṯj](https://oraec.github.io/corpus/148990.html) | [sty](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5724&db=1) |
| [ⲥⲧⲏⲙ](https://coptic-dictionary.org/entry.cgi?tla=C3810) (ID:C3810) | [sdm](https://oraec.github.io/corpus/149840.html) | [stem](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5742&db=1) |
| [ⲥⲧⲏⲙⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3811) (ID:C3811) | [srdm](https://oraec.github.io/corpus/139950.html) | [sꜣtm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5007&db=1) |
| [ⲥⲱⲧⲙ](https://coptic-dictionary.org/entry.cgi?tla=C3812) (ID:C3812) | [sḏm](https://oraec.github.io/corpus/150560.html) | [sḏm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5743&db=1) |
| [ⲥⲱⲧⲡ](https://coptic-dictionary.org/entry.cgi?tla=C3828) (ID:C3828) | [stp](https://oraec.github.io/corpus/854554.html) | [stpe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5735&db=1) |
| [ⲥⲁⲧⲉⲉⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3835) (ID:C3835) |  | [sttr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5770&db=1) |
| [ⲥⲧⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3840) (ID:C3840) | [sdꜣdꜣ](https://oraec.github.io/corpus/149680.html) |  |
| [ⲥⲱⲧϥ](https://coptic-dictionary.org/entry.cgi?tla=C3844) (ID:C3844) | [stf](https://oraec.github.io/corpus/148240.html) | [stf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5740&db=1) |
| [ⲥⲁⲧϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3847) (ID:C3847) |  | [sḏf.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5792&db=1) |
| [ⲥⲏⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3850) (ID:C3850) | [sw](https://oraec.github.io/corpus/854542.html) |  |
| [ⲥⲟⲩ-](https://coptic-dictionary.org/entry.cgi?tla=C3857) (ID:C3857) | [sw](https://oraec.github.io/corpus/854542.html) | [sw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5108&db=1) |
| [ⲥⲏⲟⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3858) (ID:C3858) |  | [sewꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5106&db=1) |
| [ⲥⲓⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3860) (ID:C3860) | [sbꜣ](https://oraec.github.io/corpus/131180.html) | [sw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5107&db=1) |
| [ⲥⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C3862) (ID:C3862) | [sjs](https://oraec.github.io/corpus/128520.html) |  |
| [ⲥⲟ](https://coptic-dictionary.org/entry.cgi?tla=C3863) (ID:C3863) | [sjs](https://oraec.github.io/corpus/128520.html) |  |
| [ⲥⲟⲩⲟ](https://coptic-dictionary.org/entry.cgi?tla=C3866) (ID:C3866) | [zw.t](https://oraec.github.io/corpus/129420.html) | [sw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5104&db=1) |
| [ⲥⲱⲟⲩⲃⲉⲛ](https://coptic-dictionary.org/entry.cgi?tla=C3867) (ID:C3867) | [snb](https://oraec.github.io/corpus/136970.html) | [swb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-5958&db=1) |
| [ⲥⲟⲩⲕⲏ](https://coptic-dictionary.org/entry.cgi?tla=C3868) (ID:C3868) | [sbg](https://oraec.github.io/corpus/132210.html) | [swgꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5159&db=1) |
| [ⲥⲟⲩⲉⲛ](https://coptic-dictionary.org/entry.cgi?tla=C3870) (ID:C3870) | [swn.t](https://oraec.github.io/corpus/130160.html) | [swn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5122&db=1) |
| [ⲥⲟⲟⲩⲛ](https://coptic-dictionary.org/entry.cgi?tla=C3871) (ID:C3871) |  | [swne](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5121&db=1) |
| [ⲥⲟⲟⲩⲧⲛ](https://coptic-dictionary.org/entry.cgi?tla=C3881) (ID:C3881) | [sdwn](https://oraec.github.io/corpus/149730.html) | [swtn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5166&db=1) |
| [ⲥⲟⲟⲩϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3889) (ID:C3889) | [swḥ.t](https://oraec.github.io/corpus/130630.html) | [swḥy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5143&db=1) |
| [ⲥⲱⲟⲩϩ](https://coptic-dictionary.org/entry.cgi?tla=C3890) (ID:C3890) | [sḥwi̯](https://oraec.github.io/corpus/140540.html) | [swḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5138&db=1) |
| [ⲥⲁⲭⲙⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3898) (ID:C3898) | [Sḫm.t](https://oraec.github.io/corpus/142250.html) | [Sḫmy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5521&db=1) |
| [ⲥⲓϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3899) (ID:C3899) |  | [sh̭y](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5549&db=1) |
| [ⲥⲓϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3900) (ID:C3900) | [sḫ.w](https://oraec.github.io/corpus/141440.html) | [sḫy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5502&db=1) |
| [ⲥⲱϣ](https://coptic-dictionary.org/entry.cgi?tla=C3903) (ID:C3903) | [zḫi̯](https://oraec.github.io/corpus/141400.html) | [sḫy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5495&db=1) |
| [ⲥⲁϣ](https://coptic-dictionary.org/entry.cgi?tla=C3905) (ID:C3905) | [zḫ.t](https://oraec.github.io/corpus/141420.html) | [sḫy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5505&db=1) |
| [ⲥⲁϣ](https://coptic-dictionary.org/entry.cgi?tla=C3906) (ID:C3906) | [zḫ.t](https://oraec.github.io/corpus/141420.html) | [sḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5488&db=1) |
| [ⲥⲱϣ](https://coptic-dictionary.org/entry.cgi?tla=C3910) (ID:C3910) |  | [sšey](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5593&db=1) |
| [ⲥⲁϣ](https://coptic-dictionary.org/entry.cgi?tla=C3912) (ID:C3912) |  | [sš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7894&db=1) |
| [ⲥⲱϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3918) (ID:C3918) | [sḫꜣḫ](https://oraec.github.io/corpus/141760.html) |  |
| [ⲥⲱϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3920) (ID:C3920) | [sḫ.t](https://oraec.github.io/corpus/141480.html) | [sḫ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5491&db=1) |
| [ⲥⲱϣⲙ](https://coptic-dictionary.org/entry.cgi?tla=C3922) (ID:C3922) | [šsm](https://oraec.github.io/corpus/157480.html) |  |
| [ⲥⲱϣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3928) (ID:C3928) | [sḫti̯](https://oraec.github.io/corpus/854549.html) | [sḫt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5537&db=1) |
| [ⲥⲁϣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3929) (ID:C3929) |  | [sẖt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7891&db=1) |
| [ϣⲟϣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3930) (ID:C3930) |  | [ššṱḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3088&db=1) |
| [ⲥⲁϣϥ](https://coptic-dictionary.org/entry.cgi?tla=C3931) (ID:C3931) | [sfḫ](https://oraec.github.io/corpus/133760.html) |  |
| [ⲥⲁϣϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3932) (ID:C3932) | [sfḫ](https://oraec.github.io/corpus/133760.html) |  |
| [ⲥⲓϣϥ](https://coptic-dictionary.org/entry.cgi?tla=C3934) (ID:C3934) | [sfḫ](https://oraec.github.io/corpus/133790.html) |  |
| [ⲥⲱϣϥ](https://coptic-dictionary.org/entry.cgi?tla=C3935) (ID:C3935) | [ḫsf](https://oraec.github.io/corpus/854535.html) | [ḫsf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4603&db=1) |
| [ⲥⲁϥ](https://coptic-dictionary.org/entry.cgi?tla=C3937) (ID:C3937) | [sf](https://oraec.github.io/corpus/133440.html) | [sf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5266&db=1) |
| [ⲥⲏϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3939) (ID:C3939) | [zf.t](https://oraec.github.io/corpus/133420.html) | [sfy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5269&db=1) |
| [ⲥⲏϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3940) (ID:C3940) | [zf.t](https://oraec.github.io/corpus/133420.html) | [sfy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1534&db=1) |
| [ⲥⲓϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3941) (ID:C3941) | [sfṯ](https://oraec.github.io/corpus/133990.html) | [sfy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5270&db=1) |
| [ⲥⲱⲱϥ](https://coptic-dictionary.org/entry.cgi?tla=C3943) (ID:C3943) |  | [sf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5267&db=1) |
| [ⲥⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C3951) (ID:C3951) | [sꜣḥ](https://oraec.github.io/corpus/127060.html) |  |
| [ⲥⲓϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3952) (ID:C3952) | [shꜣ](https://oraec.github.io/corpus/858549.html) | [shy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5438&db=1) |
| [ⲥⲟⲟϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3954) (ID:C3954) | [shꜣi̯](https://oraec.github.io/corpus/140090.html) |  |
| [ⲥⲟⲟϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3957) (ID:C3957) | [sꜥḥꜥ](https://oraec.github.io/corpus/129190.html) | [sꜥḥꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5093&db=1) |
| [ⲥⲟϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3959) (ID:C3959) | [sꜥḥꜥ](https://oraec.github.io/corpus/129190.html) | [sꜥḥꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5093&db=1) |
| [ⲥⲱϩ](https://coptic-dictionary.org/entry.cgi?tla=C3963) (ID:C3963) | [zẖ.y](https://oraec.github.io/corpus/143410.html) | [sh̭](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3125&db=1) |
| [ⲥⲱϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3965) (ID:C3965) | [sḫt](https://oraec.github.io/corpus/854548.html) | [swẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5151&db=1) |
| [ⲥⲁϩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C3970) (ID:C3970) | [sḫt.j](https://oraec.github.io/corpus/143190.html) | [sḫt.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5539&db=1) |
| [ⲥϩⲃⲏⲏⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3971) (ID:C3971) |  | [stp-p.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5737&db=1) |
| [ⲥϩⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3972) (ID:C3972) | [zẖꜣ](https://oraec.github.io/corpus/600375.html) | [sẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5552&db=1) |
| [ⲥⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C3981) (ID:C3981) | [zẖꜣ.w](https://oraec.github.io/corpus/855553.html) | [sẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5554&db=1) |
| [ⲥⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C3982) (ID:C3982) | [zẖꜣ.w](https://oraec.github.io/corpus/855553.html) | [sẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5554&db=1) |
| [ⲥϧⲓ](https://coptic-dictionary.org/entry.cgi?tla=C3983) (ID:C3983) | [zẖꜣ.w](https://oraec.github.io/corpus/450097.html) | [sẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5553&db=1) |
| [ⲥϩⲓⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3986) (ID:C3986) | [z.t-ḥm.t](https://oraec.github.io/corpus/125370.html) | [sḥm.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5458&db=1) |
| [ⲥⲱϩⲙ](https://coptic-dictionary.org/entry.cgi?tla=C3992) (ID:C3992) | [sẖm](https://oraec.github.io/corpus/143540.html) | [sẖm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5578&db=1) |
| [ⲥⲁϩⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3993) (ID:C3993) | [sḥn](https://oraec.github.io/corpus/140780.html) | [sḥn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5461&db=1) |
| [ⲟⲩⲉϩⲥⲁϩⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3996) (ID:C3996) |  | [wꜣḥ-sḥne](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1206&db=1) |
| [*ⲥⲁϩⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C3998) (ID:C3998) | [sḫni̯](https://oraec.github.io/corpus/851680.html) |  |
| [ⲥⲱϩⲡ](https://coptic-dictionary.org/entry.cgi?tla=C3999) (ID:C3999) | [sẖb](https://oraec.github.io/corpus/143480.html) |  |
| [ⲥⲓϩⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4001) (ID:C4001) | [sẖb.w](https://oraec.github.io/corpus/143490.html) |  |
| [ⲧ-](https://coptic-dictionary.org/entry.cgi?tla=C4003) (ID:C4003) | [tꜣ](https://oraec.github.io/corpus/851622.html) | [tꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6978&db=1) |
| [ⲧⲁ-](https://coptic-dictionary.org/entry.cgi?tla=C4006) (ID:C4006) | [tꜣ-n.t](https://oraec.github.io/corpus/550052.html) | [ta](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7051&db=1) |
| [ⲧⲉ⸗](https://coptic-dictionary.org/entry.cgi?tla=C11280) (ID:C11280) | [tꜣy=](https://oraec.github.io/corpus/550046.html) | [tꜣy=](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7044&db=1) |
| [ⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4007) (ID:C4007) | [tꜣj](https://oraec.github.io/corpus/851662.html) | [tꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7039&db=1) |
| [ⲧⲏ](https://coptic-dictionary.org/entry.cgi?tla=C4010) (ID:C4010) | [tr](https://oraec.github.io/corpus/172700.html) | [tꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6982&db=1) |
| [ⲧⲏ](https://coptic-dictionary.org/entry.cgi?tla=C4017) (ID:C4017) | [dwꜣ.t](https://oraec.github.io/corpus/854583.html) | [dwꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7137&db=1) |
| [ⲧⲏ](https://coptic-dictionary.org/entry.cgi?tla=C4018) (ID:C4018) | [dy](https://oraec.github.io/corpus/177830.html) | [dy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7086&db=1) |
| [ⲧⲏ](https://coptic-dictionary.org/entry.cgi?tla=C4019) (ID:C4019) | [tꜣj](https://oraec.github.io/corpus/851662.html) | [tꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7038&db=1) |
| [ϯ](https://coptic-dictionary.org/entry.cgi?tla=C4020) (ID:C4020) | [rḏi̯](https://oraec.github.io/corpus/851711.html) | [dy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7055&db=1) |
| [ϯ](https://coptic-dictionary.org/entry.cgi?tla=C4050) (ID:C4050) |  | [dy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4812&db=1) |
| [ⲧⲟ](https://coptic-dictionary.org/entry.cgi?tla=C4065) (ID:C4065) | [tꜣ](https://oraec.github.io/corpus/854573.html) | [tꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6979&db=1) |
| [ⲧⲟⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4066) (ID:C4066) | [dnj.t](https://oraec.github.io/corpus/179800.html) | [dny.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7328&db=1) |
| [ⲧⲟⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4070) (ID:C4070) | [tj.t](https://oraec.github.io/corpus/169790.html) | [ṱyꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7518&db=1) |
| [ⲧⲟⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4071) (ID:C4071) | [tj.t](https://oraec.github.io/corpus/169790.html) | [ṱyꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7518&db=1) |
| [ⲧⲱ⸗](https://coptic-dictionary.org/entry.cgi?tla=C4073) (ID:C4073) | [tꜣy=](https://oraec.github.io/corpus/550046.html) | [tꜣy=](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7044&db=1) |
| [ⲧⲃⲁ](https://coptic-dictionary.org/entry.cgi?tla=C4075) (ID:C4075) | [ḏbꜥ](https://oraec.github.io/corpus/183450.html) | [tbꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7198&db=1) |
| [ⲧⲉⲃⲓ](https://coptic-dictionary.org/entry.cgi?tla=C4078) (ID:C4078) |  | [ḏbꜥ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7218&db=1) |
| [ⲧⲉⲃⲓ](https://coptic-dictionary.org/entry.cgi?tla=C4079) (ID:C4079) |  | [ḏbꜥ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7218&db=1) |
| [ⲧⲉⲃⲓ](https://coptic-dictionary.org/entry.cgi?tla=C4080) (ID:C4080) | [ḏbꜣ](https://oraec.github.io/corpus/183240.html) | [tyb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7094&db=1) |
| [ⲧⲏⲏⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4081) (ID:C4081) | [ḏbꜥ](https://oraec.github.io/corpus/183430.html) | [ḏbꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7196&db=1) |
| [ⲧⲱⲱⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4084) (ID:C4084) | [ḏb.t](https://oraec.github.io/corpus/183120.html) | [db.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7170&db=1) |
| [ⲧⲱⲱⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4085) (ID:C4085) | [ḏb.t](https://oraec.github.io/corpus/183120.html) | [db.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7170&db=1) |
| [ⲧⲱⲱⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4086) (ID:C4086) | [ḏbꜥ](https://oraec.github.io/corpus/183460.html) | [ḏbꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7197&db=1) |
| [ⲧⲃⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4092) (ID:C4092) | [ḏbꜥ.wt](https://oraec.github.io/corpus/183530.html) |  |
| [ⲧⲱⲱⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4093) (ID:C4093) | [ḏbꜣ](https://oraec.github.io/corpus/854590.html) | [ḏbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7178&db=1) |
| [ⲧⲃⲁⲓ-](https://coptic-dictionary.org/entry.cgi?tla=C4105) (ID:C4105) | [tp.j](https://oraec.github.io/corpus/171450.html) |  |
| [ⲧⲃⲏⲗ](https://coptic-dictionary.org/entry.cgi?tla=C4107) (ID:C4107) | [dbn](https://oraec.github.io/corpus/178580.html) | [tbl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4793&db=1) |
| [ⲧⲃⲛⲏ](https://coptic-dictionary.org/entry.cgi?tla=C4109) (ID:C4109) | [tp-n-ꜥw.t](https://oraec.github.io/corpus/850078.html) | [tp-n-jꜣw.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7244&db=1) |
| [ⲧⲃⲏⲣ](https://coptic-dictionary.org/entry.cgi?tla=C4115) (ID:C4115) |  | [mꜣṱbꜣl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2316&db=1) |
| [ϯⲃⲥ](https://coptic-dictionary.org/entry.cgi?tla=C4122) (ID:C4122) | [tbs](https://oraec.github.io/corpus/170750.html) | [tbs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7224&db=1) |
| [ⲧⲃⲧ](https://coptic-dictionary.org/entry.cgi?tla=C4130) (ID:C4130) |  | [tbṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7228&db=1) |
| [ⲧⲱⲃϩ](https://coptic-dictionary.org/entry.cgi?tla=C4143) (ID:C4143) | [dbḥ](https://oraec.github.io/corpus/178750.html) | [dbḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7207&db=1) |
| [ⲧⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C4149) (ID:C4149) | [dy](https://oraec.github.io/corpus/177830.html) | [dy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7086&db=1) |
| [ⲧⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C4150) (ID:C4150) | [tꜣj](https://oraec.github.io/corpus/851662.html) | [tꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7038&db=1) |
| [ϯⲏ](https://coptic-dictionary.org/entry.cgi?tla=C4151) (ID:C4151) | [tj.t](https://oraec.github.io/corpus/169790.html) |  |
| [ⲧⲁⲓⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4166) (ID:C4166) | [ṯb](https://oraec.github.io/corpus/175070.html) | [tby.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7194&db=1) |
| [ⲧⲁⲓⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4167) (ID:C4167) | [ṯb](https://oraec.github.io/corpus/175070.html) | [tby.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7194&db=1) |
| [ⲧⲁⲓⲙ](https://coptic-dictionary.org/entry.cgi?tla=C4170) (ID:C4170) |  | [ṱm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-260&db=1) |
| [ⲧⲁⲓⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4171) (ID:C4171) |  | [tym](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7098&db=1) |
| [ⲧⲟⲓⲥ](https://coptic-dictionary.org/entry.cgi?tla=C4172) (ID:C4172) |  | [tys.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-49&db=1) |
| [ⲧⲟⲉⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C4173) (ID:C4173) |  | [tyṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7109&db=1) |
| [ⲧⲟⲕ](https://coptic-dictionary.org/entry.cgi?tla=C4188) (ID:C4188) |  | [tq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7475&db=1) |
| [ⲧⲱⲕ](https://coptic-dictionary.org/entry.cgi?tla=C4204) (ID:C4204) | [tkk](https://oraec.github.io/corpus/173740.html) | [tq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7482&db=1) |
| [ⲧⲱⲕ](https://coptic-dictionary.org/entry.cgi?tla=C4211) (ID:C4211) | [tkꜣ](https://oraec.github.io/corpus/173610.html) | [tke](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7476&db=1) |
| [ϯⲕ](https://coptic-dictionary.org/entry.cgi?tla=C4219) (ID:C4219) | [tkꜣ.w](https://oraec.github.io/corpus/173620.html) | [tyq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3288&db=1) |
| [ⲧⲱⲕⲙ](https://coptic-dictionary.org/entry.cgi?tla=C4222) (ID:C4222) |  | [tqm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7470&db=1) |
| [ⲧⲱⲕⲥ](https://coptic-dictionary.org/entry.cgi?tla=C4225) (ID:C4225) | [tks](https://oraec.github.io/corpus/173710.html) | [tqs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3807&db=1) |
| [ⲧⲁⲗ](https://coptic-dictionary.org/entry.cgi?tla=C4243) (ID:C4243) | [ṯnr](https://oraec.github.io/corpus/176080.html) |  |
| [ⲧⲁⲗⲟ](https://coptic-dictionary.org/entry.cgi?tla=C4245) (ID:C4245) |  | [dy.t-ꜥl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3217&db=1) |
| [ⲧⲓⲗⲓ](https://coptic-dictionary.org/entry.cgi?tla=C4253) (ID:C4253) |  | [tlꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7375&db=1) |
| [ⲧⲱⲗⲕ](https://coptic-dictionary.org/entry.cgi?tla=C4254) (ID:C4254) |  | [ṱlg](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7550&db=1) |
| [ⲧⲉⲗⲏⲗ](https://coptic-dictionary.org/entry.cgi?tla=C4256) (ID:C4256) | [ṯrwrw](https://oraec.github.io/corpus/176330.html) | [tꜣlꜣl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-405&db=1) |
| [ⲧⲗⲟⲙ](https://coptic-dictionary.org/entry.cgi?tla=C4260) (ID:C4260) | [tnm](https://oraec.github.io/corpus/172550.html) |  |
| [ⲧⲱⲗⲙ](https://coptic-dictionary.org/entry.cgi?tla=C4261) (ID:C4261) |  | [tlb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4807&db=1) |
| [ⲧⲗϯⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4268) (ID:C4268) |  | [tltyle.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7382&db=1) |
| [ⲧⲗϯⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4269) (ID:C4269) |  | [tltyle.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7382&db=1) |
| [ⲧⲙ-](https://coptic-dictionary.org/entry.cgi?tla=C4282) (ID:C4282) | [tm](https://oraec.github.io/corpus/854578.html) | [tm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7271&db=1) |
| [ⲧⲙⲏ](https://coptic-dictionary.org/entry.cgi?tla=C4283) (ID:C4283) | [tmꜣ.yt](https://oraec.github.io/corpus/172210.html) | [tme.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3651&db=1) |
| [ϯⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4290) (ID:C4290) | [dmj](https://oraec.github.io/corpus/179330.html) | [dmy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7287&db=1) |
| [ⲧⲟⲙ](https://coptic-dictionary.org/entry.cgi?tla=C4294) (ID:C4294) | [tmꜣ](https://oraec.github.io/corpus/172150.html) | [tme](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7275&db=1) |
| [ⲧⲱⲙ](https://coptic-dictionary.org/entry.cgi?tla=C4296) (ID:C4296) | [tmm](https://oraec.github.io/corpus/172250.html) | [tm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3883&db=1) |
| [ⲧⲱⲙ](https://coptic-dictionary.org/entry.cgi?tla=C4302) (ID:C4302) | [dm](https://oraec.github.io/corpus/852332.html) | [tme](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7277&db=1) |
| [ⲧⲱⲱⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4303) (ID:C4303) | [dmj](https://oraec.github.io/corpus/179320.html) | [tme](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7274&db=1) |
| [ⲧⲱⲱⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4307) (ID:C4307) | [tmꜣ.wt](https://oraec.github.io/corpus/172200.html) |  |
| [ⲧⲱⲙⲥ](https://coptic-dictionary.org/entry.cgi?tla=C4320) (ID:C4320) | [ṯms](https://oraec.github.io/corpus/175530.html) | [tms](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7294&db=1) |
| [ⲧⲙⲉⲧ](https://coptic-dictionary.org/entry.cgi?tla=C4323) (ID:C4323) | [dmḏ](https://oraec.github.io/corpus/179430.html) | [dmḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7297&db=1) |
| [ⲧⲱⲙⲧ](https://coptic-dictionary.org/entry.cgi?tla=C4324) (ID:C4324) | [dmḏ](https://oraec.github.io/corpus/179420.html) | [tmṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7302&db=1) |
| [ⲧⲙⲧⲙ](https://coptic-dictionary.org/entry.cgi?tla=C4329) (ID:C4329) | [tmtm](https://oraec.github.io/corpus/172340.html) |  |
| [ⲧⲙⲧⲙ](https://coptic-dictionary.org/entry.cgi?tla=C4330) (ID:C4330) | [tmtm](https://oraec.github.io/corpus/172340.html) |  |
| [ⲧⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C4334) (ID:C4334) | [ṯnw](https://oraec.github.io/corpus/175840.html) | [tne](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7306&db=1) |
| [ⲧⲏⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4337) (ID:C4337) |  | [tne](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7310&db=1) |
| [ⲧⲱⲛ](https://coptic-dictionary.org/entry.cgi?tla=C4339) (ID:C4339) | [ṯnj](https://oraec.github.io/corpus/175740.html) | [tne](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7305&db=1) |
| [ⲧⲱⲛⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C4358) (ID:C4358) | [m-dwn](https://oraec.github.io/corpus/66000.html) |  |
| [ⲧⲟⲛⲧⲛ](https://coptic-dictionary.org/entry.cgi?tla=C4368) (ID:C4368) |  | [tntn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7340&db=1) |
| [ⲧⲛϩ](https://coptic-dictionary.org/entry.cgi?tla=C4378) (ID:C4378) | [ḏnḥ](https://oraec.github.io/corpus/184370.html) | [ḏnḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7767&db=1) |
| [*ⲧⲱⲛϩ](https://coptic-dictionary.org/entry.cgi?tla=C4387) (ID:C4387) | [ḏnḥ](https://oraec.github.io/corpus/184380.html) |  |
| [ⲧⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4392) (ID:C4392) | [tp.j](https://oraec.github.io/corpus/171450.html) |  |
| [ⲧⲁⲡ](https://coptic-dictionary.org/entry.cgi?tla=C4403) (ID:C4403) | [db](https://oraec.github.io/corpus/178290.html) | [tp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7233&db=1) |
| [ⲧⲁⲡ](https://coptic-dictionary.org/entry.cgi?tla=C4407) (ID:C4407) | [ṯb](https://oraec.github.io/corpus/175070.html) |  |
| [ϯⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4408) (ID:C4408) | [dp.t](https://oraec.github.io/corpus/179030.html) |  |
| [ⲧⲟⲡ](https://coptic-dictionary.org/entry.cgi?tla=C4409) (ID:C4409) |  | [tp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7234&db=1) |
| [ⲙⲉϩⲧⲱⲡ](https://coptic-dictionary.org/entry.cgi?tla=C4411) (ID:C4411) |  | [mḥ-n-tp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2613&db=1) |
| [ⲧⲱⲡ](https://coptic-dictionary.org/entry.cgi?tla=C4415) (ID:C4415) |  | [tp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7231&db=1) |
| [ⲧⲱⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4418) (ID:C4418) | [dp](https://oraec.github.io/corpus/178970.html) | [tp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7232&db=1) |
| [ϯⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4419) (ID:C4419) | [dp.t](https://oraec.github.io/corpus/179020.html) | [tpy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7252&db=1) |
| [ⲧⲁⲡⲛ](https://coptic-dictionary.org/entry.cgi?tla=C4427) (ID:C4427) | [tpnn](https://oraec.github.io/corpus/171690.html) |  |
| [ⲧⲁⲡⲣⲟ](https://coptic-dictionary.org/entry.cgi?tla=C4428) (ID:C4428) | [tp.jt-rʾ](https://oraec.github.io/corpus/171170.html) |  |
| [ⲧⲁⲡⲧ](https://coptic-dictionary.org/entry.cgi?tla=C4430) (ID:C4430) | [dbdb](https://oraec.github.io/corpus/858677.html) |  |
| [ⲧⲣⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C4432) (ID:C4432) | [ḏr.w](https://oraec.github.io/corpus/184990.html) |  |
| [ⲧⲣⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C4433) (ID:C4433) | [ḏr.w](https://oraec.github.io/corpus/184990.html) |  |
| [ⲧⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4434) (ID:C4434) | [ḏr.t](https://oraec.github.io/corpus/184660.html) | [tre.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7351&db=1) |
| [ⲧⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4435) (ID:C4435) | [ḏr.t](https://oraec.github.io/corpus/184660.html) | [tre.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7351&db=1) |
| [ⲧⲁⲣ](https://coptic-dictionary.org/entry.cgi?tla=C4440) (ID:C4440) | [ḏr.w](https://oraec.github.io/corpus/184990.html) |  |
| [ⲧⲏⲣ⸗](https://coptic-dictionary.org/entry.cgi?tla=C4445) (ID:C4445) | [r-ḏr](https://oraec.github.io/corpus/92500.html) | [ḏr=](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7343&db=1) |
| [ⲧⲱⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4452) (ID:C4452) | [ṯr.t](https://oraec.github.io/corpus/176250.html) | [twrꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7148&db=1) |
| [ⲧⲱⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4453) (ID:C4453) | [ḏr.t](https://oraec.github.io/corpus/184630.html) | [ḏr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6975&db=1) |
| [ⲛⲧⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C4485) (ID:C4485) |  | [n-ḏr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2937&db=1) |
| [ⲧⲣⲓⲙ](https://coptic-dictionary.org/entry.cgi?tla=C4493) (ID:C4493) |  | [trmws](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7365&db=1) |
| [ⲧⲱⲣⲡ](https://coptic-dictionary.org/entry.cgi?tla=C4508) (ID:C4508) |  | [ṱrp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7544&db=1) |
| [ⲧⲣⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4519) (ID:C4519) | [twr](https://oraec.github.io/corpus/854576.html) |  |
| [ⲧⲣⲓⲣ](https://coptic-dictionary.org/entry.cgi?tla=C4521) (ID:C4521) | [trr](https://oraec.github.io/corpus/172850.html) | [ṱrry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7547&db=1) |
| [ⲧⲱⲣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C4522) (ID:C4522) | [tꜣ-rd](https://oraec.github.io/corpus/169220.html) | [trt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7371&db=1) |
| [ⲧⲱⲣϣ](https://coptic-dictionary.org/entry.cgi?tla=C4529) (ID:C4529) | [dšr](https://oraec.github.io/corpus/180690.html) | [dšr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-8099&db=1) |
| [ⲧⲱⲣϣ](https://coptic-dictionary.org/entry.cgi?tla=C4530) (ID:C4530) | [dšr](https://oraec.github.io/corpus/180690.html) | [dšr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3893&db=1) |
| [ⲧⲣⲟϣ](https://coptic-dictionary.org/entry.cgi?tla=C4531) (ID:C4531) | [dšr](https://oraec.github.io/corpus/180690.html) | [dšr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-8099&db=1) |
| [ⲧⲱⲥ](https://coptic-dictionary.org/entry.cgi?tla=C4553) (ID:C4553) | [dꜣz](https://oraec.github.io/corpus/177780.html) |  |
| [ⲧⲁⲥⲣ](https://coptic-dictionary.org/entry.cgi?tla=C4580) (ID:C4580) | [ḏsr](https://oraec.github.io/corpus/854592.html) |  |
| [ⲧⲁⲧ](https://coptic-dictionary.org/entry.cgi?tla=C4590) (ID:C4590) | [ḏd](https://oraec.github.io/corpus/185830.html) | [ḏd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-2519&db=1) |
| [ⲧⲁⲁⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4591) (ID:C4591) | [tjtj](https://oraec.github.io/corpus/170080.html) |  |
| [ⲧⲁⲁⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4592) (ID:C4592) | [tjtj](https://oraec.github.io/corpus/170080.html) |  |
| [ⲧⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C4599) (ID:C4599) | [twt](https://oraec.github.io/corpus/170480.html) | [twtw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7156&db=1) |
| [ⲧⲟⲩⲁ](https://coptic-dictionary.org/entry.cgi?tla=C4615) (ID:C4615) | [twꜣ](https://oraec.github.io/corpus/170290.html) |  |
| [ⲧⲟⲩⲁ](https://coptic-dictionary.org/entry.cgi?tla=C4616) (ID:C4616) | [twꜣ](https://oraec.github.io/corpus/170290.html) |  |
| [ⲧⲟⲩⲱ⸗](https://coptic-dictionary.org/entry.cgi?tla=C4618) (ID:C4618) |  | [twe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7125&db=1) |
| [ϩⲁⲧⲟⲩⲱ⸗](https://coptic-dictionary.org/entry.cgi?tla=C4622) (ID:C4622) |  | [ẖr-twꜣ=](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4829&db=1) |
| [ⲧⲏⲩ](https://coptic-dictionary.org/entry.cgi?tla=C4635) (ID:C4635) | [ṯꜣw](https://oraec.github.io/corpus/174480.html) | [ṯꜣw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7638&db=1) |
| [ϯⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C4651) (ID:C4651) | [dj.w](https://oraec.github.io/corpus/177840.html) |  |
| [ⲧⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C4661) (ID:C4661) | [ḏw](https://oraec.github.io/corpus/182830.html) | [twe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7123&db=1) |
| [ⲧⲟⲟⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4668) (ID:C4668) | [ṯbw](https://oraec.github.io/corpus/175120.html) | [twꜣe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7131&db=1) |
| [ⲧⲱⲟⲩⲛ](https://coptic-dictionary.org/entry.cgi?tla=C4674) (ID:C4674) | [dwn](https://oraec.github.io/corpus/178160.html) | [dwnw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7144&db=1) |
| [ⲧⲟⲩⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C4691) (ID:C4691) | [twt](https://oraec.github.io/corpus/170470.html) | [twtw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7155&db=1) |
| [ⲧⲟⲩⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C4692) (ID:C4692) | [twt](https://oraec.github.io/corpus/170470.html) | [twtw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7155&db=1) |
| [ⲧⲟⲟⲩⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4693) (ID:C4693) | [twti̯](https://oraec.github.io/corpus/170500.html) | [twtw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7156&db=1) |
| [ⲧⲁϣ](https://coptic-dictionary.org/entry.cgi?tla=C4702) (ID:C4702) | [tḫ.w](https://oraec.github.io/corpus/173170.html) |  |
| [ⲧⲱϣ](https://coptic-dictionary.org/entry.cgi?tla=C4707) (ID:C4707) | [tꜣš](https://oraec.github.io/corpus/169660.html) | [tše](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7451&db=1) |
| [ⲧⲟϣ](https://coptic-dictionary.org/entry.cgi?tla=C4720) (ID:C4720) | [tꜣš](https://oraec.github.io/corpus/169650.html) | [tše](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7453&db=1) |
| [ⲧⲁϥ](https://coptic-dictionary.org/entry.cgi?tla=C4732) (ID:C4732) | [tf](https://oraec.github.io/corpus/171750.html) | [tfꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-206&db=1) |
| [ⲧϩⲟ](https://coptic-dictionary.org/entry.cgi?tla=C4737) (ID:C4737) | [dḥr](https://oraec.github.io/corpus/180440.html) | [dḥr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7417&db=1) |
| [ⲧⲁϩⲟ](https://coptic-dictionary.org/entry.cgi?tla=C4740) (ID:C4740) |  | [dy.t-ꜥḥꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-568&db=1) |
| [ϯϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4755) (ID:C4755) | [tḫi̯](https://oraec.github.io/corpus/173110.html) | [tẖy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7433&db=1) |
| [ⲧⲱϩ](https://coptic-dictionary.org/entry.cgi?tla=C4763) (ID:C4763) | [dḥꜣ](https://oraec.github.io/corpus/180380.html) | [dḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7407&db=1) |
| [ⲧⲱϩ](https://coptic-dictionary.org/entry.cgi?tla=C4768) (ID:C4768) |  | [tẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7430&db=1) |
| [ⲧⲱϩⲃ](https://coptic-dictionary.org/entry.cgi?tla=C4777) (ID:C4777) | [tḫb](https://oraec.github.io/corpus/173210.html) | [tḫb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7425&db=1) |
| [ϯϩⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4796) (ID:C4796) |  | [thm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7392&db=1) |
| [ⲧⲱϩⲙ](https://coptic-dictionary.org/entry.cgi?tla=C4798) (ID:C4798) | [thm](https://oraec.github.io/corpus/172980.html) | [thm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7394&db=1) |
| [ⲧⲉϩⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4814) (ID:C4814) | [dhn.t](https://oraec.github.io/corpus/180320.html) |  |
| [ⲧⲱϩⲥ](https://coptic-dictionary.org/entry.cgi?tla=C4820) (ID:C4820) | [ṯḥs](https://oraec.github.io/corpus/176760.html) | [tḥs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7420&db=1) |
| [ⲧⲁϩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C4827) (ID:C4827) | [ḏḥtj](https://oraec.github.io/corpus/185320.html) | [thth](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7405&db=1) |
| [ⲧⲁϩⲧϩ](https://coptic-dictionary.org/entry.cgi?tla=C4828) (ID:C4828) | [tḫtḫ](https://oraec.github.io/corpus/173370.html) | [tẖtẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-8050&db=1) |
| [ⲧⲁϭ](https://coptic-dictionary.org/entry.cgi?tla=C4852) (ID:C4852) |  | [tyk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7106&db=1) |
| [ⲧⲁϭ](https://coptic-dictionary.org/entry.cgi?tla=C4853) (ID:C4853) |  | [tyk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7106&db=1) |
| [ϯϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4855) (ID:C4855) | [dqr](https://oraec.github.io/corpus/180950.html) | [tgy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7499&db=1) |
| [ⲧⲱⲱϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4858) (ID:C4858) | [dqr](https://oraec.github.io/corpus/854588.html) | [tgy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7497&db=1) |
| [ϭⲁⲓⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4864) (ID:C4864) | [gꜣi̯](https://oraec.github.io/corpus/166130.html) | [gꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6679&db=1) |
| [ⲧⲏϭⲙⲉⲥ](https://coptic-dictionary.org/entry.cgi?tla=C4867) (ID:C4867) | [dgm](https://oraec.github.io/corpus/181210.html) | [tgm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7500&db=1) |
| [ⲧⲱϭⲛ](https://coptic-dictionary.org/entry.cgi?tla=C4868) (ID:C4868) | [tkn](https://oraec.github.io/corpus/173680.html) | [tkn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7487&db=1) |
| [ⲧⲱϭⲣ](https://coptic-dictionary.org/entry.cgi?tla=C4870) (ID:C4870) | [dqr](https://oraec.github.io/corpus/854588.html) |  |
| [ⲧⲱϭⲥ](https://coptic-dictionary.org/entry.cgi?tla=C4872) (ID:C4872) | [dgs](https://oraec.github.io/corpus/181250.html) |  |
| [ⲧⲁϭⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4873) (ID:C4873) |  | [tks.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7495&db=1) |
| [*ⲧⲟϭⲧϭ](https://coptic-dictionary.org/entry.cgi?tla=C4879) (ID:C4879) | [dgdg](https://oraec.github.io/corpus/181270.html) |  |
| [ⲟⲩ-](https://coptic-dictionary.org/entry.cgi?tla=C4880) (ID:C4880) | [wꜥ](https://oraec.github.io/corpus/600041.html) | [wꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1256&db=1) |
| [ⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C4883) (ID:C4883) | [=w](https://oraec.github.io/corpus/42370.html) | [=w](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1172&db=1) |
| [ⲟⲩⲁ](https://coptic-dictionary.org/entry.cgi?tla=C4884) (ID:C4884) | [wꜥꜣ](https://oraec.github.io/corpus/44310.html) | [wꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7701&db=1) |
| [ⲟⲩⲁ](https://coptic-dictionary.org/entry.cgi?tla=C4894) (ID:C4894) | [wꜥ](https://oraec.github.io/corpus/600041.html) | [wꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1256&db=1) |
| [ⲟⲩⲁ](https://coptic-dictionary.org/entry.cgi?tla=C4895) (ID:C4895) | [wꜥ](https://oraec.github.io/corpus/600041.html) | [wꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1256&db=1) |
| [ⲟⲩⲁ](https://coptic-dictionary.org/entry.cgi?tla=C4896) (ID:C4896) | [wꜥ](https://oraec.github.io/corpus/600041.html) | [wꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1256&db=1) |
| [ⲟⲩⲁ-](https://coptic-dictionary.org/entry.cgi?tla=C4899) (ID:C4899) | [wꜣi̯](https://oraec.github.io/corpus/42550.html) | [wy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1228&db=1) |
| [ⲟⲩⲁ⸗](https://coptic-dictionary.org/entry.cgi?tla=C4900) (ID:C4900) | [wꜣi̯](https://oraec.github.io/corpus/42550.html) | [wy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1228&db=1) |
| [ⲟⲩⲁⲁ⸗](https://coptic-dictionary.org/entry.cgi?tla=C4901) (ID:C4901) | [wꜥ.tj](https://oraec.github.io/corpus/44230.html) | [wꜥ.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1265&db=1) |
| [ⲟⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4902) (ID:C4902) | [wꜣi̯](https://oraec.github.io/corpus/42550.html) | [wy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1228&db=1) |
| [ⲟⲩⲱ](https://coptic-dictionary.org/entry.cgi?tla=C4904) (ID:C4904) | [wꜣḥ](https://oraec.github.io/corpus/43010.html) | [wꜣḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1192&db=1) |
| [ⲟⲩⲱ](https://coptic-dictionary.org/entry.cgi?tla=C4910) (ID:C4910) | [wꜣḥ](https://oraec.github.io/corpus/43010.html) | [wꜣḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1196&db=1) |
| [ⲟⲩⲱ](https://coptic-dictionary.org/entry.cgi?tla=C4911) (ID:C4911) | [wꜣḥ](https://oraec.github.io/corpus/43010.html) | [wꜣḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1187&db=1) |
| [ⲟⲩⲱ](https://coptic-dictionary.org/entry.cgi?tla=C4921) (ID:C4921) | [wꜣḥ](https://oraec.github.io/corpus/43010.html) | [wꜣḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1187&db=1) |
| [ⲟⲩⲃⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C4927) (ID:C4927) |  | [wbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1305&db=1) |
| [ⲟⲩⲃⲁⲥⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4928) (ID:C4928) | [Bꜣs.tjt](https://oraec.github.io/corpus/53640.html) | [Bꜣs.tt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1640&db=1) |
| [ⲟⲩⲃⲁϣ](https://coptic-dictionary.org/entry.cgi?tla=C4929) (ID:C4929) | [wbḫ](https://oraec.github.io/corpus/45270.html) | [wbḫe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1317&db=1) |
| [ⲟⲩⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C4936) (ID:C4936) | [wꜣ.w](https://oraec.github.io/corpus/42630.html) | [wy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1229&db=1) |
| [ⲟⲩⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C4937) (ID:C4937) | [wꜣ.w](https://oraec.github.io/corpus/42630.html) | [wy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1229&db=1) |
| [ⲟⲩⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C4938) (ID:C4938) | [wꜣ.t](https://oraec.github.io/corpus/42490.html) | [wy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-690&db=1) |
| [ⲟⲩⲟⲉⲓⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4948) (ID:C4948) |  | [wyꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1233&db=1) |
| [ⲟⲩⲟⲉⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C4955) (ID:C4955) |  | [wyn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1237&db=1) |
| [ⲟⲩⲉⲉⲓⲉⲛⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C4963) (ID:C4963) |  | [Wynn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1241&db=1) |
| [ⲟⲩⲉⲉⲓⲉⲛⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C4964) (ID:C4964) |  | [Wynn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1241&db=1) |
| [ⲟⲩⲟⲉⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C4966) (ID:C4966) | [wḏ](https://oraec.github.io/corpus/51990.html) | [wyt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1249&db=1) |
| [ⲟⲩⲟⲉⲓϣ](https://coptic-dictionary.org/entry.cgi?tla=C4967) (ID:C4967) |  | [wš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1524&db=1) |
| [ⲟⲩⲟⲩⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4980) (ID:C4980) | [wgi̯](https://oraec.github.io/corpus/50790.html) |  |
| [ⲟⲩⲱⲱⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4982) (ID:C4982) | [wꜥr](https://oraec.github.io/corpus/44680.html) | [wle](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-972&db=1) |
| [ⲃⲗⲁⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4984) (ID:C4984) |  | [wlꜥlꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1460&db=1) |
| [ⲟⲩⲗⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4988) (ID:C4988) |  | [wl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1456&db=1) |
| [ⲟⲩⲁⲗⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C4993) (ID:C4993) | [wrm.t](https://oraec.github.io/corpus/47850.html) |  |
| [ⲟⲩⲱⲗⲡ](https://coptic-dictionary.org/entry.cgi?tla=C4994) (ID:C4994) | [wnp](https://oraec.github.io/corpus/46600.html) | [wrp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1431&db=1) |
| [ⲟⲩⲱⲗⲥ](https://coptic-dictionary.org/entry.cgi?tla=C4996) (ID:C4996) |  | [wrs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1438&db=1) |
| [ⲟⲩⲱⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5003) (ID:C5003) | [wnm](https://oraec.github.io/corpus/46710.html) | [wnm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1383&db=1) |
| [ⲟⲩⲙⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5033) (ID:C5033) | [wmt](https://oraec.github.io/corpus/45920.html) | [wmty](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1348&db=1) |
| [ⲟⲩⲟⲙⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5035) (ID:C5035) | [wmt.t](https://oraec.github.io/corpus/45990.html) | [wmte.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1349&db=1) |
| [ⲟⲩⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C5038) (ID:C5038) | [wnn](https://oraec.github.io/corpus/46050.html) | [wn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1355&db=1) |
| [ⲟⲩⲛⲧⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C5039) (ID:C5039) |  | [wn-mtw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1363&db=1) |
| [ⲟⲩⲛⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C5040) (ID:C5040) | [wnw.t](https://oraec.github.io/corpus/46420.html) | [wnw.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1378&db=1) |
| [ⲛⲧⲉⲟⲩⲛⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C5041) (ID:C5041) | [m-tꜣ-wnw.t](https://oraec.github.io/corpus/65930.html) | [twnw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7146&db=1) |
| [ⲟⲩⲁⲛ](https://coptic-dictionary.org/entry.cgi?tla=C5053) (ID:C5053) |  | [wn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1358&db=1) |
| [ⲟⲩⲉⲓⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5055) (ID:C5055) | [wni̯](https://oraec.github.io/corpus/46280.html) | [wyn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1239&db=1) |
| [ⲟⲩⲟⲛ](https://coptic-dictionary.org/entry.cgi?tla=C5057) (ID:C5057) | [wnn](https://oraec.github.io/corpus/46050.html) | [wn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1354&db=1) |
| [ⲟⲩⲱⲛ](https://coptic-dictionary.org/entry.cgi?tla=C5064) (ID:C5064) | [wn](https://oraec.github.io/corpus/46060.html) | [wn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1356&db=1) |
| [ⲟⲩⲱⲛ](https://coptic-dictionary.org/entry.cgi?tla=C5071) (ID:C5071) |  | [wn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1359&db=1) |
| [ⲟⲩⲛⲁⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5073) (ID:C5073) | [wnm.j](https://oraec.github.io/corpus/46790.html) | [wnmy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4313&db=1) |
| [ⲟⲩⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5078) (ID:C5078) | [wnḏ.wt](https://oraec.github.io/corpus/47220.html) | [wnṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1404&db=1) |
| [ⲟⲩⲱⲛϣ](https://coptic-dictionary.org/entry.cgi?tla=C5079) (ID:C5079) | [wnš](https://oraec.github.io/corpus/47020.html) | [wnš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1396&db=1) |
| [ⲟⲩⲛⲟϥ](https://coptic-dictionary.org/entry.cgi?tla=C5080) (ID:C5080) | [wnf](https://oraec.github.io/corpus/46660.html) | [wnf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1382&db=1) |
| [ⲟⲩⲉⲛⲟϥⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5086) (ID:C5086) | [Wnn-nfr](https://oraec.github.io/corpus/850648.html) | [Wn-nfr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1370&db=1) |
| [ⲟⲩⲱⲛϩ](https://coptic-dictionary.org/entry.cgi?tla=C5087) (ID:C5087) |  | [wnḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1393&db=1) |
| [ⲟⲩⲟⲡ](https://coptic-dictionary.org/entry.cgi?tla=C5096) (ID:C5096) | [wꜥb](https://oraec.github.io/corpus/44430.html) | [wꜥb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1274&db=1) |
| [ⲟⲩⲁⲁⲃ](https://coptic-dictionary.org/entry.cgi?tla=C5098) (ID:C5098) | [wꜥb](https://oraec.github.io/corpus/44430.html) | [wꜥb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1274&db=1) |
| [ⲟⲩⲏⲏⲃ](https://coptic-dictionary.org/entry.cgi?tla=C5102) (ID:C5102) | [wꜥb](https://oraec.github.io/corpus/44460.html) | [wꜥb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1276&db=1) |
| [ⲟⲩⲱⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5105) (ID:C5105) | [wbꜣ](https://oraec.github.io/corpus/44910.html) | [wbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1308&db=1) |
| [ⲟⲩⲣⲱ](https://coptic-dictionary.org/entry.cgi?tla=C5109) (ID:C5109) | [jwr.yt](https://oraec.github.io/corpus/22980.html) | [wrꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1426&db=1) |
| [ⲟⲩⲏⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5110) (ID:C5110) | [wr](https://oraec.github.io/corpus/47271.html) | [wr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1407&db=1) |
| [ⲟⲩⲏⲣ](https://coptic-dictionary.org/entry.cgi?tla=C5113) (ID:C5113) | [wr](https://oraec.github.io/corpus/47310.html) |  |
| [ⲟⲩⲱⲣⲡ](https://coptic-dictionary.org/entry.cgi?tla=C5122) (ID:C5122) |  | [wrp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1431&db=1) |
| [ⲟⲩⲣⲁⲥ](https://coptic-dictionary.org/entry.cgi?tla=C5131) (ID:C5131) | [wrs](https://oraec.github.io/corpus/48090.html) | [wrs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1441&db=1) |
| [ⲟⲩⲣⲓⲥ](https://coptic-dictionary.org/entry.cgi?tla=C5132) (ID:C5132) |  | [wrs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1439&db=1) |
| [ⲟⲩⲣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5133) (ID:C5133) |  | [wrṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1451&db=1) |
| [ⲟⲩⲣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5134) (ID:C5134) |  | [wrṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1451&db=1) |
| [ⲟⲩⲣⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5136) (ID:C5136) | [rwḏ](https://oraec.github.io/corpus/93780.html) | [rd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3601&db=1) |
| [ⲟⲩⲉⲣⲏⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5139) (ID:C5139) | [wꜥr.t](https://oraec.github.io/corpus/44740.html) |  |
| [ⲟⲩⲱⲣϩ](https://coptic-dictionary.org/entry.cgi?tla=C5144) (ID:C5144) |  | [wrḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1434&db=1) |
| [ⲟⲩⲣⲉϩ](https://coptic-dictionary.org/entry.cgi?tla=C5148) (ID:C5148) |  | [wrḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1435&db=1) |
| [ⲟⲩⲥ](https://coptic-dictionary.org/entry.cgi?tla=C5149) (ID:C5149) | [jꜣs](https://oraec.github.io/corpus/20900.html) |  |
| [ⲟⲩⲉⲓⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5154) (ID:C5154) | [wsi̯](https://oraec.github.io/corpus/49470.html) | [ws](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1506&db=1) |
| [ⲟⲩⲥⲓⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5161) (ID:C5161) | [Wsjr](https://oraec.github.io/corpus/49460.html) | [Wsjr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1502&db=1) |
| [ⲟⲩⲟⲥⲣ](https://coptic-dictionary.org/entry.cgi?tla=C5163) (ID:C5163) | [wsr](https://oraec.github.io/corpus/49620.html) | [wsr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1512&db=1) |
| [ⲟⲩⲟⲥⲧⲛ](https://coptic-dictionary.org/entry.cgi?tla=C5166) (ID:C5166) | [wsṯn](https://oraec.github.io/corpus/50030.html) | [wstn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1521&db=1) |
| [ⲟⲩⲱⲥϥ](https://coptic-dictionary.org/entry.cgi?tla=C5170) (ID:C5170) | [wzf](https://oraec.github.io/corpus/49520.html) | [wsf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1508&db=1) |
| [ⲟⲩⲁⲥϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5174) (ID:C5174) | [wzf.t](https://oraec.github.io/corpus/650064.html) |  |
| [ⲟⲩⲧⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C5175) (ID:C5175) | [r-jwd](https://oraec.github.io/corpus/91940.html) | [jwṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=433&db=1) |
| [ⲟⲩⲏⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5177) (ID:C5177) |  | [wt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1559&db=1) |
| [ⲟⲩⲏⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5178) (ID:C5178) |  | [wty](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1566&db=1) |
| [ⲟⲩⲉⲓⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5181) (ID:C5181) |  | [wty](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1566&db=1) |
| [ⲟⲩⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5183) (ID:C5183) | [wꜣḏ](https://oraec.github.io/corpus/43580.html) | [wt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-379&db=1) |
| [ⲟⲩⲟⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5184) (ID:C5184) | [wꜣḏ.t](https://oraec.github.io/corpus/43700.html) | [wt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1557&db=1) |
| [ⲟⲩⲟⲧⲟⲩⲉⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5188) (ID:C5188) | [wꜣḏwꜣḏ](https://oraec.github.io/corpus/43940.html) | [wtwt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1570&db=1) |
| [ⲟⲩⲟⲧⲟⲩⲉⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5189) (ID:C5189) | [wꜣḏwꜣḏ](https://oraec.github.io/corpus/43950.html) |  |
| [ⲟⲩⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5190) (ID:C5190) | [wꜥ.tj](https://oraec.github.io/corpus/44230.html) | [wꜥ.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1265&db=1) |
| [ⲟⲩⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5194) (ID:C5194) | [wḏꜥ](https://oraec.github.io/corpus/52360.html) | [wd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1552&db=1) |
| [ⲟⲩⲱⲧ-](https://coptic-dictionary.org/entry.cgi?tla=C5201) (ID:C5201) |  | [wṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1588&db=1) |
| [ⲟⲩⲱⲧⲃ](https://coptic-dictionary.org/entry.cgi?tla=C5203) (ID:C5203) | [wḏb](https://oraec.github.io/corpus/52620.html) | [wtb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1572&db=1) |
| [ⲟⲩⲱⲧⲛ](https://coptic-dictionary.org/entry.cgi?tla=C5218) (ID:C5218) | [wdn](https://oraec.github.io/corpus/854506.html) | [wdn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3983&db=1) |
| [ⲟⲩⲱⲧⲉⲛ](https://coptic-dictionary.org/entry.cgi?tla=C5223) (ID:C5223) | [wtn](https://oraec.github.io/corpus/51170.html) |  |
| [ⲟⲩⲱⲧϥ](https://coptic-dictionary.org/entry.cgi?tla=C5225) (ID:C5225) | [wft](https://oraec.github.io/corpus/45900.html) | [wtf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1577&db=1) |
| [ⲟⲩⲁⲧϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5226) (ID:C5226) |  | [wtf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1576&db=1) |
| [ⲟⲩⲧⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C5229) (ID:C5229) |  | [wtḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1583&db=1) |
| [ⲟⲩⲱⲧϩ](https://coptic-dictionary.org/entry.cgi?tla=C5241) (ID:C5241) | [wdḥ](https://oraec.github.io/corpus/854504.html) |  |
| [ⲟⲩⲟⲧϩ](https://coptic-dictionary.org/entry.cgi?tla=C5247) (ID:C5247) | [wdḥ.w](https://oraec.github.io/corpus/51900.html) | [wtḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1585&db=1) |
| [ⲟⲩⲟⲧϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5248) (ID:C5248) | [wdḥ.w](https://oraec.github.io/corpus/51900.html) | [wtḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1585&db=1) |
| [ⲟⲩϣⲏ](https://coptic-dictionary.org/entry.cgi?tla=C5253) (ID:C5253) | [wḫ](https://oraec.github.io/corpus/49060.html) | [wh̭](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1488&db=1) |
| [ⲟⲩⲉϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5255) (ID:C5255) |  | [wše](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1526&db=1) |
| [ⲟⲩⲱϣ](https://coptic-dictionary.org/entry.cgi?tla=C5257) (ID:C5257) | [wḫꜣ](https://oraec.github.io/corpus/49120.html) | [wḫꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1490&db=1) |
| [ⲟⲩⲱϣ](https://coptic-dictionary.org/entry.cgi?tla=C5263) (ID:C5263) |  | [wš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1524&db=1) |
| [ⲛⲟⲩⲉϣ ⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C5267) (ID:C5267) |  | [n-wš-n](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2884&db=1) |
| [ⲟⲩⲱϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5268) (ID:C5268) | [wšꜥ](https://oraec.github.io/corpus/50270.html) | [wše](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1528&db=1) |
| [ⲟⲩⲱϣⲃ](https://coptic-dictionary.org/entry.cgi?tla=C5269) (ID:C5269) | [wšb](https://oraec.github.io/corpus/50340.html) | [wšb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1535&db=1) |
| [ⲟⲩⲱϣⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5273) (ID:C5273) | [wšm](https://oraec.github.io/corpus/50540.html) | [ꜣwšm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=54&db=1) |
| [ⲟⲩϣⲁⲡ](https://coptic-dictionary.org/entry.cgi?tla=C5276) (ID:C5276) | [wšb.yt](https://oraec.github.io/corpus/50480.html) | [wšyp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1532&db=1) |
| [ⲟⲩⲁϣⲉⲣ](https://coptic-dictionary.org/entry.cgi?tla=C5279) (ID:C5279) | [wḫr.t](https://oraec.github.io/corpus/49330.html) | [wh̭r.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-6720&db=1) |
| [ⲟⲩⲱϣⲥ](https://coptic-dictionary.org/entry.cgi?tla=C5280) (ID:C5280) | [wsḫ](https://oraec.github.io/corpus/49800.html) | [wsh̭](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1514&db=1) |
| [ⲟⲩⲁϣⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5284) (ID:C5284) | [wsḫ.t](https://oraec.github.io/corpus/49850.html) | [wsh̭.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1515&db=1) |
| [ⲟⲩⲱϣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5285) (ID:C5285) | [wšd](https://oraec.github.io/corpus/50700.html) | [wšde](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1538&db=1) |
| [ⲟⲩⲁϣⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5289) (ID:C5289) |  | [wšde.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1539&db=1) |
| [ⲟⲩⲟϣⲟⲩⲉϣ](https://coptic-dictionary.org/entry.cgi?tla=C5290) (ID:C5290) | [wšwš](https://oraec.github.io/corpus/50310.html) |  |
| [ⲟⲩⲟϥ](https://coptic-dictionary.org/entry.cgi?tla=C5294) (ID:C5294) | [wfꜣ](https://oraec.github.io/corpus/45860.html) | [wef](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1346&db=1) |
| [ⲟⲩⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C5295) (ID:C5295) | [wꜣḥ](https://oraec.github.io/corpus/43030.html) |  |
| [ⲟⲩⲁϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5296) (ID:C5296) | [wḥꜣ.t](https://oraec.github.io/corpus/48700.html) | [Wḥy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1480&db=1) |
| [ⲟⲩⲓϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5298) (ID:C5298) | [whi̯](https://oraec.github.io/corpus/48330.html) | [why](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1473&db=1) |
| [ⲟⲩⲟⲟϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5302) (ID:C5302) | [wḥꜥ.t](https://oraec.github.io/corpus/48880.html) | [wḥe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1479&db=1) |
| [ⲟⲩⲱϩ](https://coptic-dictionary.org/entry.cgi?tla=C5304) (ID:C5304) | [wꜣḥ](https://oraec.github.io/corpus/43010.html) | [wꜣḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1187&db=1) |
| [*ⲟⲩⲱϩ](https://coptic-dictionary.org/entry.cgi?tla=C5320) (ID:C5320) | [wḥꜥ](https://oraec.github.io/corpus/48760.html) | [wꜣḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1197&db=1) |
| [ⲟⲩⲱϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5321) (ID:C5321) | [wḥꜥ](https://oraec.github.io/corpus/48790.html) | [wḥy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1478&db=1) |
| [ⲟⲩⲁϩⲃⲉϥ](https://coptic-dictionary.org/entry.cgi?tla=C5325) (ID:C5325) | [wḥwḥ](https://oraec.github.io/corpus/48980.html) | [wḥwḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-2140&db=1) |
| [ⲟⲩⲱϩⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5326) (ID:C5326) | [wḥm](https://oraec.github.io/corpus/48440.html) | [wḥm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1482&db=1) |
| [ⲟⲩϩⲟⲣ](https://coptic-dictionary.org/entry.cgi?tla=C5338) (ID:C5338) |  | [whr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1475&db=1) |
| [ⲟⲩϩⲟⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5339) (ID:C5339) |  | [wḥr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1487&db=1) |
| [ⲟⲩⲱϩⲣ](https://coptic-dictionary.org/entry.cgi?tla=C5343) (ID:C5343) | [wḫr](https://oraec.github.io/corpus/49310.html) |  |
| [ⲟⲩⲱϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5344) (ID:C5344) | [wḏꜥ](https://oraec.github.io/corpus/52360.html) |  |
| [ⲟⲩϫⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C5349) (ID:C5349) | [wḏꜣ](https://oraec.github.io/corpus/52090.html) | [wḏꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1602&db=1) |
| [ⲟⲩⲟϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5355) (ID:C5355) | [wg.wt](https://oraec.github.io/corpus/50840.html) | [wgy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-2563&db=1) |
| [ⲟⲩⲱϭⲡ](https://coptic-dictionary.org/entry.cgi?tla=C5359) (ID:C5359) | [wgp](https://oraec.github.io/corpus/50860.html) | [wgp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1546&db=1) |
| [ⲟⲩⲱϭⲥ](https://coptic-dictionary.org/entry.cgi?tla=C5364) (ID:C5364) | [wgs](https://oraec.github.io/corpus/50900.html) |  |
| [ⲟⲩⲟϭⲟⲩⲉϭ](https://coptic-dictionary.org/entry.cgi?tla=C5366) (ID:C5366) |  | [wgwg](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-2756&db=1) |
| [ⲫⲓⲏ](https://coptic-dictionary.org/entry.cgi?tla=C5368) (ID:C5368) | [pr.t](https://oraec.github.io/corpus/60310.html) | [pr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1989&db=1) |
| [ⲫⲉⲗ](https://coptic-dictionary.org/entry.cgi?tla=C5369) (ID:C5369) | [prj](https://oraec.github.io/corpus/60970.html) |  |
| [ⲫⲟⲣⲥ](https://coptic-dictionary.org/entry.cgi?tla=C5381) (ID:C5381) | [pnz](https://oraec.github.io/corpus/60070.html) |  |
| [ⲫⲉϧ](https://coptic-dictionary.org/entry.cgi?tla=C5385) (ID:C5385) | [pꜣḫ](https://oraec.github.io/corpus/59190.html) |  |
| [ⲫⲱϧⲉⲛ](https://coptic-dictionary.org/entry.cgi?tla=C5387) (ID:C5387) | [pḫꜣ](https://oraec.github.io/corpus/61760.html) |  |
| [ⲭⲟⲥ](https://coptic-dictionary.org/entry.cgi?tla=C5409) (ID:C5409) | [qjs](https://oraec.github.io/corpus/159730.html) |  |
| [ⲱⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5418) (ID:C5418) | [jꜣwi̯](https://oraec.github.io/corpus/20480.html) | [jꜣw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=326&db=1) |
| [ⲱⲱ⸗](https://coptic-dictionary.org/entry.cgi?tla=C5419) (ID:C5419) | [jꜣ.t](https://oraec.github.io/corpus/20090.html) | [ꜣte.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=257&db=1) |
| [ⲱⲱ](https://coptic-dictionary.org/entry.cgi?tla=C5420) (ID:C5420) | [jwr](https://oraec.github.io/corpus/22930.html) | [jwr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=419&db=1) |
| [ⲱⲃⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5426) (ID:C5426) | [ꜣpd](https://oraec.github.io/corpus/107.html) | [jpd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=472&db=1) |
| [ⲱⲃϣ](https://coptic-dictionary.org/entry.cgi?tla=C5427) (ID:C5427) | [ꜣbḫ](https://oraec.github.io/corpus/89.html) | [ꜣbḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=84&db=1) |
| [ⲱⲕ](https://coptic-dictionary.org/entry.cgi?tla=C5438) (ID:C5438) | [ꜥq](https://oraec.github.io/corpus/41180.html) | [ꜥqe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1120&db=1) |
| [ⲱⲕⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5441) (ID:C5441) | [jꜣkb](https://oraec.github.io/corpus/21010.html) | [ꜣqm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=236&db=1) |
| [ⲱⲗ](https://coptic-dictionary.org/entry.cgi?tla=C5444) (ID:C5444) | [jnr](https://oraec.github.io/corpus/27530.html) | [ꜣl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=164&db=1) |
| [ⲱⲗ](https://coptic-dictionary.org/entry.cgi?tla=C5445) (ID:C5445) | [jꜥr](https://oraec.github.io/corpus/21770.html) | [ꜥl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1051&db=1) |
| [ⲱⲗⲕ](https://coptic-dictionary.org/entry.cgi?tla=C5465) (ID:C5465) | [ꜥrq](https://oraec.github.io/corpus/854499.html) | [ꜥlq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1062&db=1) |
| [ⲱⲗⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5471) (ID:C5471) | [ꜥnb](https://oraec.github.io/corpus/38390.html) |  |
| [ⲱⲙϫ](https://coptic-dictionary.org/entry.cgi?tla=C5493) (ID:C5493) | [ꜥmḏ](https://oraec.github.io/corpus/37990.html) |  |
| [ⲱⲛ](https://coptic-dictionary.org/entry.cgi?tla=C5494) (ID:C5494) |  | [Jwnw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=413&db=1) |
| [ⲱⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5495) (ID:C5495) | [jnr](https://oraec.github.io/corpus/27560.html) | [jny](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=572&db=1) |
| [ⲱⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5496) (ID:C5496) | [jnr](https://oraec.github.io/corpus/27560.html) | [jny](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=572&db=1) |
| [ⲱⲛⲕ](https://coptic-dictionary.org/entry.cgi?tla=C5501) (ID:C5501) | [jnq](https://oraec.github.io/corpus/27880.html) |  |
| [ⲱⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5502) (ID:C5502) | [jnq](https://oraec.github.io/corpus/27880.html) |  |
| [ⲱⲛϩ](https://coptic-dictionary.org/entry.cgi?tla=C5508) (ID:C5508) | [ꜥnḫ](https://oraec.github.io/corpus/38530.html) | [ꜥnḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=995&db=1) |
| [ⲱⲡ](https://coptic-dictionary.org/entry.cgi?tla=C5513) (ID:C5513) | [jp](https://oraec.github.io/corpus/24070.html) | [jp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=453&db=1) |
| [ⲏⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5527) (ID:C5527) | [jp.t](https://oraec.github.io/corpus/24110.html) | [jpy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=455&db=1) |
| [ⲱⲣⲃ](https://coptic-dictionary.org/entry.cgi?tla=C5535) (ID:C5535) | [jnb](https://oraec.github.io/corpus/27190.html) | [jnb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=578&db=1) |
| [ⲣⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5544) (ID:C5544) |  | [rb.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3466&db=1) |
| [ⲱⲣⲕ](https://coptic-dictionary.org/entry.cgi?tla=C5548) (ID:C5548) | [ꜥrq](https://oraec.github.io/corpus/39650.html) | [ꜥrq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1043&db=1) |
| [ⲱⲣϣ](https://coptic-dictionary.org/entry.cgi?tla=C5557) (ID:C5557) |  | [jrš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=650&db=1) |
| [ⲱⲣϣ](https://coptic-dictionary.org/entry.cgi?tla=C5558) (ID:C5558) | [ꜣšr](https://oraec.github.io/corpus/287.html) |  |
| [ⲱⲣϫ](https://coptic-dictionary.org/entry.cgi?tla=C5560) (ID:C5560) | [ꜥrḏ](https://oraec.github.io/corpus/39800.html) | [ꜥrḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1050&db=1) |
| [ⲱⲥⲕ](https://coptic-dictionary.org/entry.cgi?tla=C5565) (ID:C5565) | [jsq](https://oraec.github.io/corpus/31730.html) | [jsq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=706&db=1) |
| [ⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5570) (ID:C5570) | [ꜣṯi̯](https://oraec.github.io/corpus/335.html) |  |
| [ⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5571) (ID:C5571) | [ꜥḏ](https://oraec.github.io/corpus/41980.html) | [ꜥte](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1146&db=1) |
| [ⲱⲧⲡ](https://coptic-dictionary.org/entry.cgi?tla=C5574) (ID:C5574) | [ꜣṯp](https://oraec.github.io/corpus/340.html) | [ꜣtp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=266&db=1) |
| [ⲱⲧⲡ](https://coptic-dictionary.org/entry.cgi?tla=C5580) (ID:C5580) | [ꜣṯp](https://oraec.github.io/corpus/340.html) | [ꜣtp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=266&db=1) |
| [ⲉⲧⲡⲱ](https://coptic-dictionary.org/entry.cgi?tla=C5581) (ID:C5581) | [ꜣṯp.wt](https://oraec.github.io/corpus/325.html) | [ꜣtp.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=268&db=1) |
| [ⲱⲧϩ](https://coptic-dictionary.org/entry.cgi?tla=C5583) (ID:C5583) | [jtḥ](https://oraec.github.io/corpus/33410.html) | [ꜣtḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=279&db=1) |
| [ⲁⲑⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C5588) (ID:C5588) |  | [ꜣtḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=281&db=1) |
| [ⲱⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C5589) (ID:C5589) | [ꜣwi̯](https://oraec.github.io/corpus/49.html) |  |
| [ⲱϣ](https://coptic-dictionary.org/entry.cgi?tla=C5595) (ID:C5595) | [ꜥš](https://oraec.github.io/corpus/40890.html) | [ꜥš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1102&db=1) |
| [ⲱϣⲓ](https://coptic-dictionary.org/entry.cgi?tla=C5619) (ID:C5619) | [ꜥḫi̯](https://oraec.github.io/corpus/40570.html) | [ꜥḫy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1084&db=1) |
| [ⲱϣⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5620) (ID:C5620) | [ꜥḫm](https://oraec.github.io/corpus/40630.html) | [ꜥḫm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1086&db=1) |
| [ⲁϣⲙⲓ](https://coptic-dictionary.org/entry.cgi?tla=C5623) (ID:C5623) | [ꜥḫm](https://oraec.github.io/corpus/40640.html) |  |
| [ϣϥ](https://coptic-dictionary.org/entry.cgi?tla=C5628) (ID:C5628) | [ꜥb.w](https://oraec.github.io/corpus/36750.html) | [ꜥby](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3456&db=1) |
| [ⲱϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5629) (ID:C5629) | [ꜥfi̯](https://oraec.github.io/corpus/37240.html) | [ꜥfy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=945&db=1) |
| [ⲱϥⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5631) (ID:C5631) | [ꜥfd](https://oraec.github.io/corpus/37480.html) |  |
| [ⲓϥⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5633) (ID:C5633) | [ꜥfd](https://oraec.github.io/corpus/37480.html) |  |
| [ⲱϥⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5636) (ID:C5636) | [jfd](https://oraec.github.io/corpus/24610.html) |  |
| [ⲱϩ](https://coptic-dictionary.org/entry.cgi?tla=C5639) (ID:C5639) | [jhj](https://oraec.github.io/corpus/30160.html) | [jhy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=660&db=1) |
| [ⲱϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5640) (ID:C5640) | [ꜥḥꜥ](https://oraec.github.io/corpus/851887.html) | [ꜥḥꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1072&db=1) |
| [ⲱϩⲥ](https://coptic-dictionary.org/entry.cgi?tla=C5651) (ID:C5651) | [ꜣzḫ](https://oraec.github.io/corpus/264.html) | [ꜣsḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=223&db=1) |
| [ⲟϩⲥ](https://coptic-dictionary.org/entry.cgi?tla=C5655) (ID:C5655) | [ꜣzḫ](https://oraec.github.io/corpus/281.html) | [ꜣsẖ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=225&db=1) |
| [ⲱϫ](https://coptic-dictionary.org/entry.cgi?tla=C5659) (ID:C5659) | [jṯꜣ](https://oraec.github.io/corpus/33540.html) | [ꜣḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=287&db=1) |
| [ⲱϫⲛ](https://coptic-dictionary.org/entry.cgi?tla=C5661) (ID:C5661) |  | [ꜥḏnꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1165&db=1) |
| [ⲱϭⲃ](https://coptic-dictionary.org/entry.cgi?tla=C5666) (ID:C5666) |  | [ꜥkf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1136&db=1) |
| [ⲱϭⲃ](https://coptic-dictionary.org/entry.cgi?tla=C5667) (ID:C5667) | [ꜣgb.w](https://oraec.github.io/corpus/314.html) |  |
| [ϣ-](https://coptic-dictionary.org/entry.cgi?tla=C5673) (ID:C5673) | [rḫ](https://oraec.github.io/corpus/95620.html) | [rḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3542&db=1) |
| [ϣⲁ-](https://coptic-dictionary.org/entry.cgi?tla=C5675) (ID:C5675) | [šꜣꜥ-r](https://oraec.github.io/corpus/151540.html) | [šꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5830&db=1) |
| [ϣⲁ](https://coptic-dictionary.org/entry.cgi?tla=C5676) (ID:C5676) | [šꜣꜥ](https://oraec.github.io/corpus/851685.html) | [šꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5831&db=1) |
| [ϣⲁ](https://coptic-dictionary.org/entry.cgi?tla=C5679) (ID:C5679) | [ḫꜥi̯](https://oraec.github.io/corpus/114740.html) | [ḫꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4428&db=1) |
| [ϣⲁ](https://coptic-dictionary.org/entry.cgi?tla=C5684) (ID:C5684) | [ḫꜥ](https://oraec.github.io/corpus/114620.html) | [ḫꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-699&db=1) |
| [ϣⲁ](https://coptic-dictionary.org/entry.cgi?tla=C5691) (ID:C5691) | [šr.t](https://oraec.github.io/corpus/156610.html) | [šy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5812&db=1) |
| [ϣⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C5695) (ID:C5695) | [šꜣ.w](https://oraec.github.io/corpus/151300.html) | [šy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5814&db=1) |
| [ϣⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C5696) (ID:C5696) | [ḫ](https://oraec.github.io/corpus/112980.html) |  |
| [ϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5698) (ID:C5698) | [šmi̯](https://oraec.github.io/corpus/154340.html) | [šm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5992&db=1) |
| [ϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5699) (ID:C5699) | [ḫt](https://oraec.github.io/corpus/121200.html) | [ḫt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4610&db=1) |
| [ϩⲁⲙϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5701) (ID:C5701) |  | [ḥm-šnꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4079&db=1) |
| [ϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5704) (ID:C5704) | [šn.t](https://oraec.github.io/corpus/155320.html) |  |
| [ϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5706) (ID:C5706) | [šnꜥ.tj](https://oraec.github.io/corpus/155920.html) |  |
| [ϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5707) (ID:C5707) | [ꜥnḫ](https://oraec.github.io/corpus/38530.html) | [ꜥnḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=997&db=1) |
| [ϣⲉⲉⲓ](https://coptic-dictionary.org/entry.cgi?tla=C5709) (ID:C5709) |  | [šm-jy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6005&db=1) |
| [ϣⲏⲓ](https://coptic-dictionary.org/entry.cgi?tla=C5711) (ID:C5711) | [š](https://oraec.github.io/corpus/854557.html) | [šy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5813&db=1) |
| [ϣⲓ](https://coptic-dictionary.org/entry.cgi?tla=C5713) (ID:C5713) | [ḫꜣi̯](https://oraec.github.io/corpus/113410.html) | [ẖy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4709&db=1) |
| [ϣⲓ](https://coptic-dictionary.org/entry.cgi?tla=C5723) (ID:C5723) | [ḫꜣ.y](https://oraec.github.io/corpus/113430.html) |  |
| [ϣⲓⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C5724) (ID:C5724) | [ḫyi̯](https://oraec.github.io/corpus/114460.html) | [h̭y](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1470&db=1) |
| [ϣⲓⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C5725) (ID:C5725) | [ḫy](https://oraec.github.io/corpus/114470.html) | [h̭ꜥy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7791&db=1) |
| [ϣⲓⲏ](https://coptic-dictionary.org/entry.cgi?tla=C5726) (ID:C5726) | [ḫy](https://oraec.github.io/corpus/114470.html) | [h̭ꜥy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7791&db=1) |
| [ϣⲓⲏ](https://coptic-dictionary.org/entry.cgi?tla=C5727) (ID:C5727) | [ḫy](https://oraec.github.io/corpus/114470.html) | [h̭ꜥy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7791&db=1) |
| [ϣⲓⲏ](https://coptic-dictionary.org/entry.cgi?tla=C5728) (ID:C5728) | [ḫyi̯](https://oraec.github.io/corpus/114460.html) | [h̭y](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1470&db=1) |
| [ϣⲓⲱ](https://coptic-dictionary.org/entry.cgi?tla=C5730) (ID:C5730) |  | [h̭yꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4650&db=1) |
| [ϣⲟ](https://coptic-dictionary.org/entry.cgi?tla=C5731) (ID:C5731) | [ḫꜣ](https://oraec.github.io/corpus/113110.html) |  |
| [ϣⲟ](https://coptic-dictionary.org/entry.cgi?tla=C5732) (ID:C5732) | [m-šs](https://oraec.github.io/corpus/600392.html) | [m-šs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2254&db=1) |
| [ϣⲱ](https://coptic-dictionary.org/entry.cgi?tla=C5735) (ID:C5735) | [šꜥy](https://oraec.github.io/corpus/152280.html) | [šꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5832&db=1) |
| [ϣⲱⲓ](https://coptic-dictionary.org/entry.cgi?tla=C5738) (ID:C5738) | [ḫy](https://oraec.github.io/corpus/114470.html) | [h̭ꜥy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7791&db=1) |
| [ϣⲱⲓ](https://coptic-dictionary.org/entry.cgi?tla=C5740) (ID:C5740) | [ḫw](https://oraec.github.io/corpus/113070.html) |  |
| [ϣⲱⲃ](https://coptic-dictionary.org/entry.cgi?tla=C5742) (ID:C5742) | [ḫbi̯](https://oraec.github.io/corpus/115570.html) | [ḫby](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4450&db=1) |
| [ϣⲓⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5743) (ID:C5743) | [šbi̯](https://oraec.github.io/corpus/153350.html) | [šbe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5914&db=1) |
| [ϣⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5747) (ID:C5747) | [šf.yt](https://oraec.github.io/corpus/154080.html) | [šfeꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5975&db=1) |
| [ϣⲏⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5748) (ID:C5748) | [ḏꜥb.t](https://oraec.github.io/corpus/182660.html) | [ḏbe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7725&db=1) |
| [ϣⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5749) (ID:C5749) | [sfḫ](https://oraec.github.io/corpus/133800.html) |  |
| [ϣⲓⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5751) (ID:C5751) | [šbi̯](https://oraec.github.io/corpus/153350.html) | [šbe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5914&db=1) |
| [ϣⲃⲓⲱ](https://coptic-dictionary.org/entry.cgi?tla=C5756) (ID:C5756) | [šb.t](https://oraec.github.io/corpus/153250.html) | [šb.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5919&db=1) |
| [ϣⲃⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C5760) (ID:C5760) |  | [šbn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5928&db=1) |
| [ϣⲃⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C5761) (ID:C5761) |  | [šbn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5928&db=1) |
| [ϣⲃⲏⲣ](https://coptic-dictionary.org/entry.cgi?tla=C5764) (ID:C5764) | [ḫbr](https://oraec.github.io/corpus/115700.html) | [ḫber](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4458&db=1) |
| [ϣⲓⲃⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5767) (ID:C5767) | [šbi̯](https://oraec.github.io/corpus/153350.html) | [šbe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5914&db=1) |
| [ϣⲃⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5773) (ID:C5773) | [šbd](https://oraec.github.io/corpus/153600.html) | [šbte](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5931&db=1) |
| [ϣⲃϣⲓ](https://coptic-dictionary.org/entry.cgi?tla=C5775) (ID:C5775) | [šps.w](https://oraec.github.io/corpus/153880.html) |  |
| [ϣⲱⲃϩ](https://coptic-dictionary.org/entry.cgi?tla=C5776) (ID:C5776) |  | [šwḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5906&db=1) |
| [ϣⲁⲑⲱⲗ](https://coptic-dictionary.org/entry.cgi?tla=C5777) (ID:C5777) |  | [štl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6233&db=1) |
| [ϣⲱⲕ](https://coptic-dictionary.org/entry.cgi?tla=C5780) (ID:C5780) | [šꜣd](https://oraec.github.io/corpus/152150.html) |  |
| [ϣⲓⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5782) (ID:C5782) | [šdi̯](https://oraec.github.io/corpus/854561.html) | [šqy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1069&db=1) |
| [ϣⲓⲕ](https://coptic-dictionary.org/entry.cgi?tla=C5785) (ID:C5785) |  | [šqe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6168&db=1) |
| [ϣⲕⲗⲕⲓⲗ](https://coptic-dictionary.org/entry.cgi?tla=C5791) (ID:C5791) |  | [šqlql](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6171&db=1) |
| [ϣⲱⲕϩ](https://coptic-dictionary.org/entry.cgi?tla=C5800) (ID:C5800) |  | [šꜣkh](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5810&db=1) |
| [ϣⲁⲗ](https://coptic-dictionary.org/entry.cgi?tla=C5802) (ID:C5802) | [ḫry](https://oraec.github.io/corpus/119870.html) | [ḫr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-773&db=1) |
| [ϣⲟⲗ](https://coptic-dictionary.org/entry.cgi?tla=C5805) (ID:C5805) |  | [ḫl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4587&db=1) |
| [ϣⲟⲗ](https://coptic-dictionary.org/entry.cgi?tla=C5807) (ID:C5807) | [šꜣr.w](https://oraec.github.io/corpus/151870.html) |  |
| [ϣⲱⲗ](https://coptic-dictionary.org/entry.cgi?tla=C5808) (ID:C5808) | [ḫnr](https://oraec.github.io/corpus/118390.html) | [ḫl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4588&db=1) |
| [ϣⲱⲗ](https://coptic-dictionary.org/entry.cgi?tla=C5814) (ID:C5814) | [ḫnr](https://oraec.github.io/corpus/118390.html) | [ḫl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4588&db=1) |
| [ϣⲗⲏ](https://coptic-dictionary.org/entry.cgi?tla=C5815) (ID:C5815) | [ḫnr](https://oraec.github.io/corpus/118390.html) | [ẖlꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4890&db=1) |
| [ϣⲗⲏⲗ](https://coptic-dictionary.org/entry.cgi?tla=C5821) (ID:C5821) | [šrr](https://oraec.github.io/corpus/156840.html) | [šlle](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6123&db=1) |
| [ϣⲗⲟⲗ](https://coptic-dictionary.org/entry.cgi?tla=C5825) (ID:C5825) |  | [šll](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6121&db=1) |
| [ϣⲱⲗⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5826) (ID:C5826) | [ḫnm](https://oraec.github.io/corpus/854533.html) | [ḫnmm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4527&db=1) |
| [ϣⲱⲗⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5833) (ID:C5833) | [šrm](https://oraec.github.io/corpus/156790.html) |  |
| [ϣⲟⲗⲙⲉⲥ](https://coptic-dictionary.org/entry.cgi?tla=C5835) (ID:C5835) | [ḫnms](https://oraec.github.io/corpus/118280.html) | [ḫnms](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4530&db=1) |
| [ϣⲗⲁⲉⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C5836) (ID:C5836) |  | [ḫlyn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4593&db=1) |
| [ϣⲗⲟⲡ](https://coptic-dictionary.org/entry.cgi?tla=C5838) (ID:C5838) |  | [ḫlpe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4595&db=1) |
| [ϣⲉⲗⲉⲉⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5840) (ID:C5840) |  | [šlṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6131&db=1) |
| [ϣⲟⲗϣⲗ](https://coptic-dictionary.org/entry.cgi?tla=C5847) (ID:C5847) | [ḫrḫr](https://oraec.github.io/corpus/120420.html) | [ḫrḫr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4574&db=1) |
| [ϣⲗⲟϥ](https://coptic-dictionary.org/entry.cgi?tla=C5851) (ID:C5851) | [šnrf](https://oraec.github.io/corpus/156220.html) | [šlf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1076&db=1) |
| [ϣⲗⲟϥ](https://coptic-dictionary.org/entry.cgi?tla=C5852) (ID:C5852) | [šnrf](https://oraec.github.io/corpus/156220.html) | [ẖlf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1426&db=1) |
| [ϣⲗϩ](https://coptic-dictionary.org/entry.cgi?tla=C5853) (ID:C5853) |  | [šlḥe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6127&db=1) |
| [ϣⲗϩ](https://coptic-dictionary.org/entry.cgi?tla=C5854) (ID:C5854) |  | [šlḥe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6127&db=1) |
| [ϣⲗⲉϩ](https://coptic-dictionary.org/entry.cgi?tla=C5855) (ID:C5855) | [srḥ.w](https://oraec.github.io/corpus/860883.html) |  |
| [ϣⲗⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C5859) (ID:C5859) |  | [šlḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6126&db=1) |
| [ϣⲱⲗϭ](https://coptic-dictionary.org/entry.cgi?tla=C5863) (ID:C5863) | [srq](https://oraec.github.io/corpus/139770.html) |  |
| [ϣⲗⲓϭ](https://coptic-dictionary.org/entry.cgi?tla=C5864) (ID:C5864) |  | [šlṱe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-123&db=1) |
| [ϣⲗϭⲟⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5865) (ID:C5865) |  | [šlgm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6129&db=1) |
| [ϣⲗϭⲟⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5866) (ID:C5866) |  | [šlgm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6129&db=1) |
| [ϣⲏⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5869) (ID:C5869) | [ḫm](https://oraec.github.io/corpus/116910.html) | [ḫm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4499&db=1) |
| [ϣⲏⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5875) (ID:C5875) | [sšm](https://oraec.github.io/corpus/144990.html) | [šm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-509&db=1) |
| [ϣⲟⲉⲓⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5878) (ID:C5878) | [šmw](https://oraec.github.io/corpus/154450.html) | [šm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-8108&db=1) |
| [ϣⲓⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5879) (ID:C5879) | [šm.t](https://oraec.github.io/corpus/154400.html) |  |
| [ϣⲟⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5880) (ID:C5880) |  | [šm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5998&db=1) |
| [ϣⲱⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5881) (ID:C5881) | [šm.t](https://oraec.github.io/corpus/154440.html) | [šm.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6011&db=1) |
| [ϣⲱⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5882) (ID:C5882) | [šꜣm.w](https://oraec.github.io/corpus/151800.html) |  |
| [ϣⲱⲙ](https://coptic-dictionary.org/entry.cgi?tla=C5883) (ID:C5883) | [šm.w](https://oraec.github.io/corpus/154850.html) | [šmw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5995&db=1) |
| [ϣⲱⲱⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5887) (ID:C5887) | [jḫm.t](https://oraec.github.io/corpus/30870.html) |  |
| [ϣⲙⲁ](https://coptic-dictionary.org/entry.cgi?tla=C5888) (ID:C5888) | [šmꜥ](https://oraec.github.io/corpus/154710.html) | [šmꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6025&db=1) |
| [ϣⲱⲱⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5890) (ID:C5890) | [šmꜥ](https://oraec.github.io/corpus/154720.html) |  |
| [ϣⲙⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C5891) (ID:C5891) |  | [šmw.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6032&db=1) |
| [ϣⲙⲙⲟ](https://coptic-dictionary.org/entry.cgi?tla=C5893) (ID:C5893) | [šmꜣ](https://oraec.github.io/corpus/154570.html) | [šmꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6024&db=1) |
| [ϣⲙⲙⲟ](https://coptic-dictionary.org/entry.cgi?tla=C5895) (ID:C5895) |  | [šmꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6024&db=1) |
| [ϣⲙⲟⲩⲛ](https://coptic-dictionary.org/entry.cgi?tla=C5903) (ID:C5903) | [ḫmn](https://oraec.github.io/corpus/117240.html) |  |
| [ϣⲟⲙⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5905) (ID:C5905) | [ḫmt.w](https://oraec.github.io/corpus/117280.html) | [ḫmt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4512&db=1) |
| [ϣⲙϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5909) (ID:C5909) | [šms](https://oraec.github.io/corpus/155000.html) | [šmsy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6042&db=1) |
| [ϣⲙϣⲏϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5915) (ID:C5915) |  | [šmšeke](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6045&db=1) |
| [ϣⲏⲛ](https://coptic-dictionary.org/entry.cgi?tla=C5917) (ID:C5917) | [šn](https://oraec.github.io/corpus/155240.html) | [šn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6050&db=1) |
| [ϣⲓⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5922) (ID:C5922) | [šni̯](https://oraec.github.io/corpus/854559.html) | [šn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6054&db=1) |
| [ϣⲱⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5936) (ID:C5936) | [šni̯](https://oraec.github.io/corpus/155480.html) | [šny](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6055&db=1) |
| [ϣⲱⲱⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5940) (ID:C5940) | [šnꜥ](https://oraec.github.io/corpus/854560.html) | [šnꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6071&db=1) |
| [ϣⲛⲁ](https://coptic-dictionary.org/entry.cgi?tla=C5943) (ID:C5943) | [šnꜥ.w](https://oraec.github.io/corpus/155880.html) | [šnꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6072&db=1) |
| [ϣⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5945) (ID:C5945) | [šn.w](https://oraec.github.io/corpus/155940.html) | [šne](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6060&db=1) |
| [ϣⲛⲏ](https://coptic-dictionary.org/entry.cgi?tla=C5947) (ID:C5947) | [šn.wj](https://oraec.github.io/corpus/156000.html) | [šn.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6062&db=1) |
| [ϣⲛⲥ](https://coptic-dictionary.org/entry.cgi?tla=C5948) (ID:C5948) | [sšr.w-nswt](https://oraec.github.io/corpus/850993.html) | [šs-n-nsw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6146&db=1) |
| [ϣⲉⲛⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5949) (ID:C5949) | [šnṯ.y](https://oraec.github.io/corpus/156470.html) |  |
| [ϣⲱⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5950) (ID:C5950) | [ḫnd](https://oraec.github.io/corpus/119430.html) |  |
| [ϣⲱⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C5953) (ID:C5953) | [šnṯ](https://oraec.github.io/corpus/156400.html) | [ḫnṱe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4545&db=1) |
| [ϣⲟⲛⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5957) (ID:C5957) | [šnḏ.t](https://oraec.github.io/corpus/156510.html) | [šnte.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6087&db=1) |
| [ϣⲛⲧⲱ](https://coptic-dictionary.org/entry.cgi?tla=C5959) (ID:C5959) | [šnḏ.wt](https://oraec.github.io/corpus/156540.html) | [šnt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6086&db=1) |
| [ϣⲛⲟϣ](https://coptic-dictionary.org/entry.cgi?tla=C5961) (ID:C5961) | [ḫnš](https://oraec.github.io/corpus/118730.html) | [ḫnš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4535&db=1) |
| [ϣⲛⲟϣ](https://coptic-dictionary.org/entry.cgi?tla=C5962) (ID:C5962) | [ḫnš](https://oraec.github.io/corpus/118730.html) | [ḫnš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4535&db=1) |
| [ϣⲱⲛϥ](https://coptic-dictionary.org/entry.cgi?tla=C5964) (ID:C5964) | [šbn](https://oraec.github.io/corpus/153490.html) | [šbn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5926&db=1) |
| [ϣⲛϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5966) (ID:C5966) | [šnf.t](https://oraec.github.io/corpus/156140.html) | [ḫnfy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4526&db=1) |
| [ϣⲁⲡ](https://coptic-dictionary.org/entry.cgi?tla=C5967) (ID:C5967) |  | [šp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5942&db=1) |
| [ϣⲟⲡ](https://coptic-dictionary.org/entry.cgi?tla=C5969) (ID:C5969) | [šzp](https://oraec.github.io/corpus/157200.html) | [šsp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6148&db=1) |
| [ϣⲱⲡ](https://coptic-dictionary.org/entry.cgi?tla=C5971) (ID:C5971) | [šzp](https://oraec.github.io/corpus/157160.html) | [šsp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5935&db=1) |
| [ϣⲱⲡ](https://coptic-dictionary.org/entry.cgi?tla=C5981) (ID:C5981) | [šby.w](https://oraec.github.io/corpus/153370.html) | [šp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5941&db=1) |
| [ϣⲱⲡ](https://coptic-dictionary.org/entry.cgi?tla=C5982) (ID:C5982) | [sšp](https://oraec.github.io/corpus/144860.html) | [šp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5939&db=1) |
| [ϣⲓⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5986) (ID:C5986) | [špt](https://oraec.github.io/corpus/153970.html) | [špy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5943&db=1) |
| [ϣⲱⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C5995) (ID:C5995) | [ḫpr](https://oraec.github.io/corpus/854383.html) | [ḫpr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4467&db=1) |
| [ϣⲱⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6002) (ID:C6002) | [sšp.t](https://oraec.github.io/corpus/144920.html) | [špy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5958&db=1) |
| [ϣⲱⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6003) (ID:C6003) | [sšp.t](https://oraec.github.io/corpus/144920.html) | [špy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5958&db=1) |
| [ϣⲡⲏⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6006) (ID:C6006) | [ḫpr.t](https://oraec.github.io/corpus/116270.html) | [ḫpry.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4471&db=1) |
| [ϣⲡⲏⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6007) (ID:C6007) | [ḫpr.t](https://oraec.github.io/corpus/116270.html) | [ḫpry.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4471&db=1) |
| [ϣⲱⲡϣ](https://coptic-dictionary.org/entry.cgi?tla=C6011) (ID:C6011) | [ḫpš](https://oraec.github.io/corpus/116430.html) | [ḫpš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4473&db=1) |
| [ϣⲁⲣ-](https://coptic-dictionary.org/entry.cgi?tla=C6014) (ID:C6014) | [šrr](https://oraec.github.io/corpus/156570.html) |  |
| [ϣⲁⲁⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6015) (ID:C6015) | [ḫꜥr](https://oraec.github.io/corpus/600161.html) | [ḫꜥr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4437&db=1) |
| [ϣⲁⲁⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6019) (ID:C6019) | [šꜥr](https://oraec.github.io/corpus/152550.html) | [šꜥr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5859&db=1) |
| [ϣⲱⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6024) (ID:C6024) | [šrj](https://oraec.github.io/corpus/156670.html) |  |
| [ϣⲁⲣⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C6025) (ID:C6025) | [ḫr](https://oraec.github.io/corpus/400037.html) | [ḫr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4549&db=1) |
| [ϣⲁⲁⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6026) (ID:C6026) | [ḫꜥr](https://oraec.github.io/corpus/114890.html) | [ḫꜥry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4435&db=1) |
| [ϣⲁⲓⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6030) (ID:C6030) | [sḏr.yt](https://oraec.github.io/corpus/150820.html) | [sḏr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5761&db=1) |
| [ϣⲏⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6032) (ID:C6032) | [šrj](https://oraec.github.io/corpus/156650.html) | [šr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6091&db=1) |
| [ϣⲉⲉⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6033) (ID:C6033) | [šrj.t](https://oraec.github.io/corpus/156680.html) | [šre.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6093&db=1) |
| [ϣⲓⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6043) (ID:C6043) | [šrr](https://oraec.github.io/corpus/156820.html) |  |
| [ϣⲓⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6047) (ID:C6047) | [šrj](https://oraec.github.io/corpus/156660.html) |  |
| [ϣⲱⲣⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6055) (ID:C6055) | [ḫrp](https://oraec.github.io/corpus/120150.html) | [ḫrp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4568&db=1) |
| [ϣⲟⲣⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6058) (ID:C6058) |  | [ḫrp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1398&db=1) |
| [ϣⲟⲣⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6059) (ID:C6059) |  | [ḫrp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1398&db=1) |
| [ϣⲟⲣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6064) (ID:C6064) | [ḫrd](https://oraec.github.io/corpus/120500.html) | [ḫrṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4583&db=1) |
| [ϣⲟⲣϣⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6069) (ID:C6069) | [ḫrḫr](https://oraec.github.io/corpus/120420.html) | [ḫrḫr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4574&db=1) |
| [ϣⲱⲣϫ](https://coptic-dictionary.org/entry.cgi?tla=C6072) (ID:C6072) |  | [ḫrḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4584&db=1) |
| [ϣⲱⲥ](https://coptic-dictionary.org/entry.cgi?tla=C6074) (ID:C6074) | [Šꜣs.w](https://oraec.github.io/corpus/151930.html) | [šs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4353&db=1) |
| [ϣⲥⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6077) (ID:C6077) | [zḫn](https://oraec.github.io/corpus/142460.html) | [sḫny](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5528&db=1) |
| [ϣⲥⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6079) (ID:C6079) | [ṯz.w](https://oraec.github.io/corpus/176900.html) |  |
| [ϣⲟⲉⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6080) (ID:C6080) | [ḫꜣt](https://oraec.github.io/corpus/113800.html) | [ḫyṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4426&db=1) |
| [ϣⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6082) (ID:C6082) | [šd](https://oraec.github.io/corpus/158470.html) | [šd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6209&db=1) |
| [ϣⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6084) (ID:C6084) | [šwy.tj](https://oraec.github.io/corpus/153090.html) | [šwṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5897&db=1) |
| [ϣⲱⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6089) (ID:C6089) | [šꜥḏ](https://oraec.github.io/corpus/450452.html) | [šꜥd.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5872&db=1) |
| [ϣⲁⲁⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6094) (ID:C6094) |  | [šꜥd.ṱ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5875&db=1) |
| [ϣⲁⲁⲧⲥ](https://coptic-dictionary.org/entry.cgi?tla=C6095) (ID:C6095) |  | [šꜥd.ṱ=s](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5871&db=1) |
| [ϣⲓⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6099) (ID:C6099) | [šdi̯](https://oraec.github.io/corpus/854561.html) | [šdy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-783&db=1) |
| [ϣⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6101) (ID:C6101) | [šd.t](https://oraec.github.io/corpus/158600.html) | [šdy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6221&db=1) |
| [ϣⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6102) (ID:C6102) | [šḏ.t](https://oraec.github.io/corpus/158970.html) |  |
| [ϣⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6104) (ID:C6104) | [ḫt-ṯꜣ.w](https://oraec.github.io/corpus/121460.html) | [ḫt-ṯꜣw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4612&db=1) |
| [ϣⲱⲧⲃ](https://coptic-dictionary.org/entry.cgi?tla=C6107) (ID:C6107) | [štb](https://oraec.github.io/corpus/158290.html) |  |
| [ϣⲧⲟⲃ](https://coptic-dictionary.org/entry.cgi?tla=C6108) (ID:C6108) | [štb](https://oraec.github.io/corpus/158300.html) |  |
| [ϣⲧⲉⲕⲟ](https://coptic-dictionary.org/entry.cgi?tla=C6109) (ID:C6109) |  | [štqy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6237&db=1) |
| [ϣⲱⲧⲙ](https://coptic-dictionary.org/entry.cgi?tla=C6112) (ID:C6112) | [ḫtm](https://oraec.github.io/corpus/121710.html) | [ḫtm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4633&db=1) |
| [ϣⲧⲁⲙ](https://coptic-dictionary.org/entry.cgi?tla=C6113) (ID:C6113) | [ḫtm](https://oraec.github.io/corpus/121710.html) | [ḫtm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4633&db=1) |
| [ϣⲧⲟⲙ](https://coptic-dictionary.org/entry.cgi?tla=C6114) (ID:C6114) | [ḫtm](https://oraec.github.io/corpus/121730.html) | [ḫtm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4634&db=1) |
| [ϣⲧⲏⲛ](https://coptic-dictionary.org/entry.cgi?tla=C6118) (ID:C6118) |  | [gtwn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3481&db=1) |
| [ϣϯⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6129) (ID:C6129) | [sḫt.j](https://oraec.github.io/corpus/143190.html) | [sḫt.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5539&db=1) |
| [ϣⲧⲟⲩⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6130) (ID:C6130) |  | [šṱwṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6241&db=1) |
| [ϣⲟⲧϣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6131) (ID:C6131) |  | [štšt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6236&db=1) |
| [ϣⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6133) (ID:C6133) | [šꜣ.w](https://oraec.github.io/corpus/151310.html) | [šw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5877&db=1) |
| [ϣⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6134) (ID:C6134) | [šꜣ.w](https://oraec.github.io/corpus/151560.html) | [šw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5876&db=1) |
| [ϣⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6139) (ID:C6139) | [šꜣ.w](https://oraec.github.io/corpus/151560.html) | [šw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5876&db=1) |
| [ϣⲟⲩ-](https://coptic-dictionary.org/entry.cgi?tla=C6140) (ID:C6140) | [šꜣ.w](https://oraec.github.io/corpus/151560.html) | [šw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5876&db=1) |
| [ϣⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6141) (ID:C6141) | [šꜣ.w](https://oraec.github.io/corpus/151310.html) | [šw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5877&db=1) |
| [ϣⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6142) (ID:C6142) | [šꜣ](https://oraec.github.io/corpus/151120.html) |  |
| [ⲛϣⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6145) (ID:C6145) | [šwi̯](https://oraec.github.io/corpus/152670.html) |  |
| [ϣⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6146) (ID:C6146) | [ḫꜣ.w](https://oraec.github.io/corpus/113330.html) | [ḫwy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4447&db=1) |
| [ϣⲏⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6148) (ID:C6148) | [ḫꜣw.t](https://oraec.github.io/corpus/113720.html) | [ḫwy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4444&db=1) |
| [ϣⲟⲟⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6149) (ID:C6149) | [šwi̯](https://oraec.github.io/corpus/152720.html) | [šw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5884&db=1) |
| [ϣⲟⲩⲟ](https://coptic-dictionary.org/entry.cgi?tla=C6150) (ID:C6150) | [sšwi̯](https://oraec.github.io/corpus/144810.html) |  |
| [ϣⲟⲩⲏⲃ](https://coptic-dictionary.org/entry.cgi?tla=C6154) (ID:C6154) | [šwb](https://oraec.github.io/corpus/153110.html) | [šwꜣbꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5903&db=1) |
| [ϣⲟⲩⲱⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6155) (ID:C6155) | [šbb](https://oraec.github.io/corpus/153410.html) |  |
| [ϣⲟⲩⲥⲟⲟⲩϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6157) (ID:C6157) |  | [swšy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5155&db=1) |
| [ϣⲟⲩϣⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6161) (ID:C6161) | [sꜥšꜣ](https://oraec.github.io/corpus/129260.html) | [šꜥš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5864&db=1) |
| [ϣⲟⲉⲓϣ](https://coptic-dictionary.org/entry.cgi?tla=C6168) (ID:C6168) |  | [šꜥyḫ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5856&db=1) |
| [ϣⲟϣ](https://coptic-dictionary.org/entry.cgi?tla=C6169) (ID:C6169) | [šsꜣ](https://oraec.github.io/corpus/157080.html) | [šš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-498&db=1) |
| [ϣⲟϣ](https://coptic-dictionary.org/entry.cgi?tla=C6170) (ID:C6170) | [šsꜣ](https://oraec.github.io/corpus/157080.html) | [šš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-498&db=1) |
| [ϣⲱϣ](https://coptic-dictionary.org/entry.cgi?tla=C6172) (ID:C6172) | [ḫꜣḫꜣ](https://oraec.github.io/corpus/114220.html) | [šše](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6151&db=1) |
| [ϣⲱϣ](https://coptic-dictionary.org/entry.cgi?tla=C6175) (ID:C6175) | [šš](https://oraec.github.io/corpus/157750.html) | [šš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6152&db=1) |
| [ϣⲁϣϥ](https://coptic-dictionary.org/entry.cgi?tla=C6176) (ID:C6176) | [ḫsf](https://oraec.github.io/corpus/450465.html) |  |
| [ϣⲟⲩϣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6183) (ID:C6183) | [sšd](https://oraec.github.io/corpus/145880.html) | [ššte](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6163&db=1) |
| [ϣⲟϣⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6185) (ID:C6185) |  | [ššw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6154&db=1) |
| [ϣⲁϥ](https://coptic-dictionary.org/entry.cgi?tla=C6188) (ID:C6188) | [ḫfꜣꜣ.t](https://oraec.github.io/corpus/116620.html) | [ḫfꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4483&db=1) |
| [ϣⲱϥ](https://coptic-dictionary.org/entry.cgi?tla=C6189) (ID:C6189) | [fḫ](https://oraec.github.io/corpus/63970.html) | [ḫf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4480&db=1) |
| [ϣⲱⲱϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6192) (ID:C6192) |  | [šfꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5979&db=1) |
| [ϣⲁϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6193) (ID:C6193) | [šfu̯](https://oraec.github.io/corpus/154160.html) |  |
| [ϣϥⲱ](https://coptic-dictionary.org/entry.cgi?tla=C6196) (ID:C6196) |  | [sḫfꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5514&db=1) |
| [ϣϥⲱ](https://coptic-dictionary.org/entry.cgi?tla=C6197) (ID:C6197) |  | [sh̭fe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5513&db=1) |
| [ϣⲱϥⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6199) (ID:C6199) |  | [šft](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5982&db=1) |
| [ϣⲟϥⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6200) (ID:C6200) |  | [šft](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5986&db=1) |
| [ϣⲁϥⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6202) (ID:C6202) | [ḫft.j](https://oraec.github.io/corpus/116800.html) | [ḫft](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4484&db=1) |
| [ϣⲱϥⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6204) (ID:C6204) | [šfd](https://oraec.github.io/corpus/154280.html) |  |
| [ϣϩⲓϭ](https://coptic-dictionary.org/entry.cgi?tla=C6215) (ID:C6215) | [šḥq](https://oraec.github.io/corpus/156900.html) | [ẖqe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4910&db=1) |
| [ϣⲁϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6216) (ID:C6216) | [sḏd](https://oraec.github.io/corpus/150940.html) | [sḏy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5785&db=1) |
| [ϣⲱϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6225) (ID:C6225) |  | [sḏy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5786&db=1) |
| [ϣϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6231) (ID:C6231) |  | [sḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5781&db=1) |
| [ϣϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6232) (ID:C6232) |  | [šk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6173&db=1) |
| [ϣϫⲏⲛ](https://coptic-dictionary.org/entry.cgi?tla=C6235) (ID:C6235) |  | [ḫḏn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4646&db=1) |
| [ϣⲟϫⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6236) (ID:C6236) | [sṯni̯](https://oraec.github.io/corpus/854556.html) | [sḏny](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5794&db=1) |
| [ϣⲱϫⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6241) (ID:C6241) | [sḏb](https://oraec.github.io/corpus/150440.html) | [sḏm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-8081&db=1) |
| [ϣⲱⲱϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6246) (ID:C6246) | [sqr](https://oraec.github.io/corpus/854551.html) | [škꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6178&db=1) |
| [ϣϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6250) (ID:C6250) | [sgꜣ](https://oraec.github.io/corpus/147120.html) |  |
| [ϣϭⲛⲏⲛ](https://coptic-dictionary.org/entry.cgi?tla=C6252) (ID:C6252) |  | [šgnn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7660&db=1) |
| [ϣϭⲁⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6254) (ID:C6254) | [sgb](https://oraec.github.io/corpus/147160.html) | [sgpe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5687&db=1) |
| [ϣϭⲟⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6256) (ID:C6256) |  | [škr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6181&db=1) |
| [ϥ](https://coptic-dictionary.org/entry.cgi?tla=C11282) (ID:C11282) | [=f](https://oraec.github.io/corpus/10050.html) | [=f](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2193&db=1) |
| [ϥⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6260) (ID:C6260) | [fꜣi̯](https://oraec.github.io/corpus/63460.html) | [fy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2197&db=1) |
| [ϥⲟ](https://coptic-dictionary.org/entry.cgi?tla=C6268) (ID:C6268) |  | [fꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2207&db=1) |
| [ϥⲱ](https://coptic-dictionary.org/entry.cgi?tla=C6269) (ID:C6269) | [fꜥy](https://oraec.github.io/corpus/852956.html) | [fꜥe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2206&db=1) |
| [ϥⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6276) (ID:C6276) | [fnṯ](https://oraec.github.io/corpus/63890.html) |  |
| [ϥⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6277) (ID:C6277) | [fnṯ](https://oraec.github.io/corpus/63890.html) |  |
| [ϥⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6282) (ID:C6282) | [fdi̯](https://oraec.github.io/corpus/64280.html) | [fty](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2218&db=1) |
| [ϥⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6284) (ID:C6284) | [fd.t](https://oraec.github.io/corpus/64260.html) | [ftyꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2219&db=1) |
| [ϥⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6285) (ID:C6285) | [fd.t](https://oraec.github.io/corpus/64260.html) | [ftyꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2219&db=1) |
| [ϥⲧⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6289) (ID:C6289) | [jfd.w](https://oraec.github.io/corpus/850571.html) | [jfṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=479&db=1) |
| [ϥⲱϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6291) (ID:C6291) | [fqꜣ](https://oraec.github.io/corpus/64040.html) |  |
| [ⳉⲟ](https://coptic-dictionary.org/entry.cgi?tla=C6295) (ID:C6295) | [ḫꜣ](https://oraec.github.io/corpus/113230.html) |  |
| [ⳉⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6299) (ID:C6299) | [ḫt.w](https://oraec.github.io/corpus/121610.html) | [ḫtꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4622&db=1) |
| [ϧⲁ](https://coptic-dictionary.org/entry.cgi?tla=C6304) (ID:C6304) | [ḫr](https://oraec.github.io/corpus/850795.html) | [h̭ꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3108&db=1) |
| [ϧⲏⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6310) (ID:C6310) | [šw](https://oraec.github.io/corpus/152750.html) | [šw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5882&db=1) |
| [ϧⲉⲛⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6317) (ID:C6317) | [ẖnn](https://oraec.github.io/corpus/123700.html) | [ẖnyny](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7667&db=1) |
| [ϧⲱⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6318) (ID:C6318) | [ḫr](https://oraec.github.io/corpus/119610.html) | [ẖr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4807&db=1) |
| [ϧⲣⲟϯ](https://coptic-dictionary.org/entry.cgi?tla=C6321) (ID:C6321) | [ẖrd](https://oraec.github.io/corpus/854539.html) | [ẖrd.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4870&db=1) |
| [ϧⲱⲥ](https://coptic-dictionary.org/entry.cgi?tla=C6323) (ID:C6323) | [ẖz](https://oraec.github.io/corpus/124610.html) | [ẖsy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7962&db=1) |
| [ϧⲁϧ](https://coptic-dictionary.org/entry.cgi?tla=C6326) (ID:C6326) | [ḫḫ](https://oraec.github.io/corpus/120510.html) | [ẖẖe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4903&db=1) |
| [ϧⲱϧ](https://coptic-dictionary.org/entry.cgi?tla=C6327) (ID:C6327) | [ḫꜣḫ](https://oraec.github.io/corpus/114170.html) |  |
| [ϩⲁ-](https://coptic-dictionary.org/entry.cgi?tla=C6328) (ID:C6328) | [ẖr](https://oraec.github.io/corpus/850794.html) | [ẖr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4797&db=1) |
| [ϩⲁ-](https://coptic-dictionary.org/entry.cgi?tla=C6333) (ID:C6333) | [ḫr](https://oraec.github.io/corpus/850795.html) | [h̭ꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3108&db=1) |
| [ϩⲁ](https://coptic-dictionary.org/entry.cgi?tla=C6336) (ID:C6336) |  | [ẖꜥy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4733&db=1) |
| [ϩⲁⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6338) (ID:C6338) | [ḫꜣꜥ](https://oraec.github.io/corpus/862789.html) | [ẖꜥꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-860&db=1) |
| [ϩⲁⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6339) (ID:C6339) | [ḫꜣꜥ](https://oraec.github.io/corpus/862789.html) | [ẖꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4731&db=1) |
| [ϩⲁⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6340) (ID:C6340) |  | [ẖꜥ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4729&db=1) |
| [ϩⲁⲏ](https://coptic-dictionary.org/entry.cgi?tla=C6348) (ID:C6348) |  | [ḥꜣe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3939&db=1) |
| [ϩⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6349) (ID:C6349) | [hj](https://oraec.github.io/corpus/97770.html) | [hy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3734&db=1) |
| [ϩⲁⲓⲟ](https://coptic-dictionary.org/entry.cgi?tla=C6353) (ID:C6353) | [hy](https://oraec.github.io/corpus/97760.html) | [hy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3730&db=1) |
| [ϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6354) (ID:C6354) | [hꜣi̯](https://oraec.github.io/corpus/97350.html) | [hy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3732&db=1) |
| [ϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6360) (ID:C6360) | [ẖ.t](https://oraec.github.io/corpus/122080.html) | [ẖ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4686&db=1) |
| [ϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6369) (ID:C6369) | [ḥꜣ](https://oraec.github.io/corpus/100160.html) |  |
| [ϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6370) (ID:C6370) | [ḥꜣ](https://oraec.github.io/corpus/854528.html) | [ḥe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3928&db=1) |
| [ϩⲏ](https://coptic-dictionary.org/entry.cgi?tla=C6372) (ID:C6372) | [ḥꜣ.t](https://oraec.github.io/corpus/100310.html) | [ḥꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1087&db=1) |
| [ϩⲏⲧ⸗](https://coptic-dictionary.org/entry.cgi?tla=C6373) (ID:C6373) |  | [ḥꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3933&db=1) |
| [ⲉⲑⲏ](https://coptic-dictionary.org/entry.cgi?tla=C6375) (ID:C6375) |  | [r-tꜣ-ḥꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1473&db=1) |
| [ϩⲏ](https://coptic-dictionary.org/entry.cgi?tla=C6381) (ID:C6381) | [ẖ.t](https://oraec.github.io/corpus/122080.html) | [ẖe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4683&db=1) |
| [ⲛϩⲏⲧ⸗](https://coptic-dictionary.org/entry.cgi?tla=C6382) (ID:C6382) |  | [n-ẖ.t-n](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2903&db=1) |
| [ϩⲏ](https://coptic-dictionary.org/entry.cgi?tla=C6383) (ID:C6383) | [ẖ.t](https://oraec.github.io/corpus/122080.html) | [ẖe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4683&db=1) |
| [ϩⲏ](https://coptic-dictionary.org/entry.cgi?tla=C6385) (ID:C6385) | [hꜣw](https://oraec.github.io/corpus/854526.html) | [hꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3723&db=1) |
| [ϩⲓⲏ](https://coptic-dictionary.org/entry.cgi?tla=C6394) (ID:C6394) | [ḥr.t](https://oraec.github.io/corpus/107660.html) |  |
| [ϩⲟ](https://coptic-dictionary.org/entry.cgi?tla=C6398) (ID:C6398) | [ḥr](https://oraec.github.io/corpus/107510.html) | [ḥr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4155&db=1) |
| [ϫⲓ ϩⲣⲁ⸗](https://coptic-dictionary.org/entry.cgi?tla=C6406) (ID:C6406) |  | [sḏyḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5787&db=1) |
| [ⲉϩⲣⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C6409) (ID:C6409) | [r-ḥr](https://oraec.github.io/corpus/92210.html) | [r-ḥr-n](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3381&db=1) |
| [ⲛⲁϩⲣⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C6410) (ID:C6410) | [m-ḥr](https://oraec.github.io/corpus/65170.html) | [n-j.jr-ḥr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2917&db=1) |
| [ϩⲓϩⲣⲁ⸗](https://coptic-dictionary.org/entry.cgi?tla=C6411) (ID:C6411) |  | [ḥr-ḥr n](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4188&db=1) |
| [ϩⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6413) (ID:C6413) | [ḥꜣy.t](https://oraec.github.io/corpus/100770.html) |  |
| [ϩⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6414) (ID:C6414) | [ḥꜣ.t](https://oraec.github.io/corpus/100260.html) | [ḥyyt.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3958&db=1) |
| [ϩⲱ](https://coptic-dictionary.org/entry.cgi?tla=C6419) (ID:C6419) | [ḥw.t](https://oraec.github.io/corpus/99790.html) | [ḥ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3897&db=1) |
| [ϩⲱⲱ⸗](https://coptic-dictionary.org/entry.cgi?tla=C6420) (ID:C6420) | [ḥꜥ.w](https://oraec.github.io/corpus/854529.html) | [ḥꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3971&db=1) |
| [ϩⲓⲉⲓⲃ](https://coptic-dictionary.org/entry.cgi?tla=C6422) (ID:C6422) |  | [ḥyb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3960&db=1) |
| [ϩⲓⲉⲓⲃ](https://coptic-dictionary.org/entry.cgi?tla=C6423) (ID:C6423) |  | [ḥyb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3960&db=1) |
| [ϩⲱⲃ](https://coptic-dictionary.org/entry.cgi?tla=C6424) (ID:C6424) | [hꜣb](https://oraec.github.io/corpus/97580.html) | [hb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3781&db=1) |
| [ϩⲏⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6435) (ID:C6435) | [ḥb](https://oraec.github.io/corpus/851405.html) | [ḥbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4021&db=1) |
| [ϩⲏⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6436) (ID:C6436) | [ḥb](https://oraec.github.io/corpus/851405.html) | [ḥbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4021&db=1) |
| [ϩⲓⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6439) (ID:C6439) | [hbu̯](https://oraec.github.io/corpus/98020.html) | [hbe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3786&db=1) |
| [ϩⲓⲃⲱⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6442) (ID:C6442) | [hbj](https://oraec.github.io/corpus/98120.html) | [hb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3783&db=1) |
| [ϩⲃⲁ](https://coptic-dictionary.org/entry.cgi?tla=C6443) (ID:C6443) | [ḥb](https://oraec.github.io/corpus/851405.html) | [ḥbꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4021&db=1) |
| [ϩⲃⲱ](https://coptic-dictionary.org/entry.cgi?tla=C6446) (ID:C6446) | [ḥꜣb](https://oraec.github.io/corpus/103290.html) | [ḥbꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4019&db=1) |
| [ϩⲃⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6447) (ID:C6447) | [hbu̯](https://oraec.github.io/corpus/98010.html) |  |
| [ϩⲱⲃⲕ](https://coptic-dictionary.org/entry.cgi?tla=C6448) (ID:C6448) | [hbq](https://oraec.github.io/corpus/98220.html) |  |
| [ϩⲃⲟⲩⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6450) (ID:C6450) |  | [gbyr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6771&db=1) |
| [ϩⲃⲟⲣⲃⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6451) (ID:C6451) | [ḥbnbn](https://oraec.github.io/corpus/103690.html) | [hbrbre](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3794&db=1) |
| [ϩⲁⲓⲃⲉⲥ](https://coptic-dictionary.org/entry.cgi?tla=C6454) (ID:C6454) | [ḫꜣyb.t](https://oraec.github.io/corpus/113540.html) | [ẖybꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-113&db=1) |
| [ϩⲏⲃⲥ](https://coptic-dictionary.org/entry.cgi?tla=C6458) (ID:C6458) | [ḫbs](https://oraec.github.io/corpus/113860.html) | [ẖbs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4754&db=1) |
| [ϩⲱⲃⲥ](https://coptic-dictionary.org/entry.cgi?tla=C6459) (ID:C6459) | [ḥbs](https://oraec.github.io/corpus/103740.html) | [ḥbs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4029&db=1) |
| [ϩⲃⲟⲟⲥ](https://coptic-dictionary.org/entry.cgi?tla=C6462) (ID:C6462) | [ḥbs](https://oraec.github.io/corpus/103750.html) | [ḥbs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4031&db=1) |
| [ϩⲃⲟⲟⲥ](https://coptic-dictionary.org/entry.cgi?tla=C6463) (ID:C6463) | [ḥbs](https://oraec.github.io/corpus/103750.html) | [ḥbs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4031&db=1) |
| [ϩⲃⲥⲱ](https://coptic-dictionary.org/entry.cgi?tla=C6464) (ID:C6464) | [ḥbs.wt](https://oraec.github.io/corpus/103920.html) | [ḥbs.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4033&db=1) |
| [ϩⲁⲕ](https://coptic-dictionary.org/entry.cgi?tla=C6469) (ID:C6469) | [ẖꜥq](https://oraec.github.io/corpus/122810.html) | [ẖꜥq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4739&db=1) |
| [ϩⲓⲕ](https://coptic-dictionary.org/entry.cgi?tla=C6471) (ID:C6471) | [ḥkꜣ.w](https://oraec.github.io/corpus/110660.html) | [ḥyq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3963&db=1) |
| [ϩⲱⲱⲕ](https://coptic-dictionary.org/entry.cgi?tla=C6474) (ID:C6474) | [ẖkr](https://oraec.github.io/corpus/124730.html) | [ẖq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4909&db=1) |
| [ϩⲁⲕⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6478) (ID:C6478) |  | [ḥq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4289&db=1) |
| [ϩⲁⲕⲟ](https://coptic-dictionary.org/entry.cgi?tla=C6479) (ID:C6479) | [ḥkꜣ.w](https://oraec.github.io/corpus/110700.html) |  |
| [ϩⲏⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6481) (ID:C6481) | [ḥqꜣ.t](https://oraec.github.io/corpus/110440.html) |  |
| [ϩⲱⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6482) (ID:C6482) | [ẖꜥq](https://oraec.github.io/corpus/122800.html) | [ẖꜥqe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4738&db=1) |
| [ϩⲁⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6484) (ID:C6484) | [ẖꜥq](https://oraec.github.io/corpus/122810.html) | [ẖꜥq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4739&db=1) |
| [ϩⲕⲟ](https://coptic-dictionary.org/entry.cgi?tla=C6486) (ID:C6486) | [ḥqr](https://oraec.github.io/corpus/110540.html) | [ḥqr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4301&db=1) |
| [ϩⲏⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6489) (ID:C6489) | [ḥqr](https://oraec.github.io/corpus/110550.html) |  |
| [ϩⲁⲗ](https://coptic-dictionary.org/entry.cgi?tla=C6498) (ID:C6498) | [ḥnr](https://oraec.github.io/corpus/106860.html) | [ḥlle](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4252&db=1) |
| [ϩⲁⲗ](https://coptic-dictionary.org/entry.cgi?tla=C6503) (ID:C6503) | [ḫr.j](https://oraec.github.io/corpus/119850.html) | [ẖl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4872&db=1) |
| [ϩⲁⲗ](https://coptic-dictionary.org/entry.cgi?tla=C6504) (ID:C6504) | [ḫr.j](https://oraec.github.io/corpus/119850.html) | [ẖl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4872&db=1) |
| [ϩⲙϩⲁⲗ](https://coptic-dictionary.org/entry.cgi?tla=C6506) (ID:C6506) |  | [ḫm-ẖl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4506&db=1) |
| [ϩⲙϩⲁⲗ](https://coptic-dictionary.org/entry.cgi?tla=C6507) (ID:C6507) |  | [ḫm-ẖl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4506&db=1) |
| [ϩⲁⲗⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6516) (ID:C6516) | [ḥri̯](https://oraec.github.io/corpus/108340.html) | [ḥl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4243&db=1) |
| [ϩⲱⲗ](https://coptic-dictionary.org/entry.cgi?tla=C6518) (ID:C6518) | [ḫnr](https://oraec.github.io/corpus/118410.html) |  |
| [ϩⲱⲗ](https://coptic-dictionary.org/entry.cgi?tla=C6519) (ID:C6519) | [ḥri̯](https://oraec.github.io/corpus/108340.html) | [ḥl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4243&db=1) |
| [ϩⲉⲗⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6525) (ID:C6525) | [ḥr.yt](https://oraec.github.io/corpus/108390.html) |  |
| [ϩⲏⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6526) (ID:C6526) | [ḥnw.t](https://oraec.github.io/corpus/106340.html) | [ḥnw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4131&db=1) |
| [ϩⲱⲱⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6532) (ID:C6532) | [ḫꜣꜥ](https://oraec.github.io/corpus/113560.html) | [ḫꜣꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4386&db=1) |
| [ϩⲱⲱⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6533) (ID:C6533) | [ḥꜣꜥꜥ](https://oraec.github.io/corpus/101010.html) |  |
| [ϩⲗⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6534) (ID:C6534) | [ḥr.w](https://oraec.github.io/corpus/107760.html) | [ḥr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4156&db=1) |
| [ϩⲗⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6535) (ID:C6535) | [ḥr.w](https://oraec.github.io/corpus/107760.html) | [ḥr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4156&db=1) |
| [ϩⲁⲗⲃϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6537) (ID:C6537) | [rbš](https://oraec.github.io/corpus/94010.html) | [lbš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3662&db=1) |
| [ϩⲁⲗⲁⲕ](https://coptic-dictionary.org/entry.cgi?tla=C6538) (ID:C6538) |  | [hlq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3861&db=1) |
| [ϩⲱⲗⲕ](https://coptic-dictionary.org/entry.cgi?tla=C6539) (ID:C6539) |  | [hlk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3865&db=1) |
| [ϩⲗⲟⲗ](https://coptic-dictionary.org/entry.cgi?tla=C6545) (ID:C6545) | [ḥnr](https://oraec.github.io/corpus/854746.html) | [ḥlle](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4252&db=1) |
| [ϩⲁⲗⲓⲗ](https://coptic-dictionary.org/entry.cgi?tla=C6547) (ID:C6547) | [ḥrr.t](https://oraec.github.io/corpus/109120.html) |  |
| [ϩⲗⲟⲉⲓⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6548) (ID:C6548) |  | [ḥlꜥlꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4247&db=1) |
| [ϩⲗⲟⲟⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6550) (ID:C6550) |  | [hlꜥlꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3855&db=1) |
| [ϩⲗⲗⲟ](https://coptic-dictionary.org/entry.cgi?tla=C6551) (ID:C6551) |  | [ẖl-ꜥꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4878&db=1) |
| [ϩⲗⲱⲙ](https://coptic-dictionary.org/entry.cgi?tla=C6560) (ID:C6560) |  | [hꜥlꜥmꜥtꜥ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3764&db=1) |
| [ϩⲗⲟⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6568) (ID:C6568) |  | [ẖrp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4862&db=1) |
| [ϩⲗⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6569) (ID:C6569) | [ẖpꜣ](https://oraec.github.io/corpus/122880.html) | [ẖlpy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4895&db=1) |
| [ϩⲁⲗⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6576) (ID:C6576) |  | [hꜥleṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3763&db=1) |
| [ϩⲟⲗϩⲗ](https://coptic-dictionary.org/entry.cgi?tla=C6582) (ID:C6582) | [ẖnẖn](https://oraec.github.io/corpus/123810.html) | [ẖlẖl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4898&db=1) |
| [ϩⲱⲗϭ](https://coptic-dictionary.org/entry.cgi?tla=C6590) (ID:C6590) |  | [ḥlg](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4258&db=1) |
| [ϩⲗⲟϭ](https://coptic-dictionary.org/entry.cgi?tla=C6591) (ID:C6591) | [ḥꜣg](https://oraec.github.io/corpus/101610.html) | [ḥlk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4257&db=1) |
| [ϩⲁⲙ](https://coptic-dictionary.org/entry.cgi?tla=C6602) (ID:C6602) | [ḥmw.w](https://oraec.github.io/corpus/105480.html) | [ḥm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4053&db=1) |
| [ϩⲟⲉⲓⲙ](https://coptic-dictionary.org/entry.cgi?tla=C6607) (ID:C6607) | [hꜣn.w](https://oraec.github.io/corpus/97670.html) | [hym](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3749&db=1) |
| [ϩⲱⲙ](https://coptic-dictionary.org/entry.cgi?tla=C6611) (ID:C6611) | [ḥm](https://oraec.github.io/corpus/104700.html) | [hm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3806&db=1) |
| [ϩⲁⲙⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6615) (ID:C6615) |  | [hmy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3810&db=1) |
| [ϩⲏⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6616) (ID:C6616) | [hm.t](https://oraec.github.io/corpus/98420.html) | [hme.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3807&db=1) |
| [ϩⲙⲏ](https://coptic-dictionary.org/entry.cgi?tla=C6624) (ID:C6624) | [ḥn.t](https://oraec.github.io/corpus/106020.html) |  |
| [ϩⲙⲏ](https://coptic-dictionary.org/entry.cgi?tla=C6625) (ID:C6625) | [ḥn.t](https://oraec.github.io/corpus/106020.html) |  |
| [ϩⲙⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6627) (ID:C6627) | [ḥmꜣ.t](https://oraec.github.io/corpus/105070.html) | [ḥmꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4085&db=1) |
| [ϩⲙⲟⲙ](https://coptic-dictionary.org/entry.cgi?tla=C6630) (ID:C6630) | [šmm](https://oraec.github.io/corpus/154890.html) | [ẖmm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4765&db=1) |
| [ϩⲙⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6632) (ID:C6632) | [šmm](https://oraec.github.io/corpus/154910.html) | [šm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5994&db=1) |
| [ϩⲙⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6633) (ID:C6633) | [šmm](https://oraec.github.io/corpus/154910.html) | [šm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5994&db=1) |
| [ϩⲙⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6634) (ID:C6634) | [ḥm.yt](https://oraec.github.io/corpus/105240.html) |  |
| [ϩⲟⲙⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6639) (ID:C6639) | [ḥmt](https://oraec.github.io/corpus/450114.html) | [ḥmt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4100&db=1) |
| [ϩⲁⲙⲏⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6644) (ID:C6644) |  | [ḥmwl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4091&db=1) |
| [ϩⲙⲥ](https://coptic-dictionary.org/entry.cgi?tla=C6647) (ID:C6647) | [ẖms](https://oraec.github.io/corpus/123010.html) | [ẖms](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4767&db=1) |
| [ϩⲙⲟⲟⲥ](https://coptic-dictionary.org/entry.cgi?tla=C6649) (ID:C6649) | [ḥmsi̯](https://oraec.github.io/corpus/105780.html) | [ḥmsy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4096&db=1) |
| [ϩⲱⲙⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6652) (ID:C6652) | [ḥm.t](https://oraec.github.io/corpus/104750.html) |  |
| [ϩⲙϩⲙ](https://coptic-dictionary.org/entry.cgi?tla=C6660) (ID:C6660) | [hmhm](https://oraec.github.io/corpus/98480.html) | [hmhm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3811&db=1) |
| [ϩⲟⲙϩⲉⲙ](https://coptic-dictionary.org/entry.cgi?tla=C6662) (ID:C6662) | [hbhb](https://oraec.github.io/corpus/98200.html) | [hbhb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3797&db=1) |
| [ϩⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C6668) (ID:C6668) | [m-ẖnw](https://oraec.github.io/corpus/65370.html) | [ẖn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4768&db=1) |
| [ϩⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C6672) (ID:C6672) | [hnw](https://oraec.github.io/corpus/98700.html) | [hn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3817&db=1) |
| [ϩⲟⲩⲛ](https://coptic-dictionary.org/entry.cgi?tla=C6676) (ID:C6676) | [ẖnw](https://oraec.github.io/corpus/854537.html) | [ẖn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-755&db=1) |
| [ⲛϩⲟⲩⲛ](https://coptic-dictionary.org/entry.cgi?tla=C6680) (ID:C6680) |  | [n-ẖn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-393&db=1) |
| [ϩⲱⲛ](https://coptic-dictionary.org/entry.cgi?tla=C6686) (ID:C6686) | [ẖn](https://oraec.github.io/corpus/123110.html) | [ẖn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4769&db=1) |
| [ϩⲱⲛ](https://coptic-dictionary.org/entry.cgi?tla=C6688) (ID:C6688) | [ḥn](https://oraec.github.io/corpus/105900.html) | [ḥn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4102&db=1) |
| [ϩⲏⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6697) (ID:C6697) |  | [ḥny.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4124&db=1) |
| [ϩⲏⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6701) (ID:C6701) | [hnw](https://oraec.github.io/corpus/98560.html) | [hn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3817&db=1) |
| [ϩⲓⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6702) (ID:C6702) | [ẖni̯](https://oraec.github.io/corpus/123230.html) | [ẖn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1031&db=1) |
| [ϩⲓⲛⲓⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6703) (ID:C6703) | [ḥmw](https://oraec.github.io/corpus/105300.html) | [ḥny](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4123&db=1) |
| [*ϩⲓⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6704) (ID:C6704) | [ḥn](https://oraec.github.io/corpus/854531.html) | [ḥn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4112&db=1) |
| [ϩⲟⲓⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6705) (ID:C6705) | [nhj](https://oraec.github.io/corpus/85370.html) | [hyn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3750&db=1) |
| [ϩⲱⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6706) (ID:C6706) | [ḥn.t](https://oraec.github.io/corpus/106050.html) | [ḥny.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4121&db=1) |
| [ϩⲛⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C6708) (ID:C6708) | [ḥn](https://oraec.github.io/corpus/105900.html) | [ḥn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4104&db=1) |
| [ϩⲟⲛⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6713) (ID:C6713) | [ẖnm.t](https://oraec.github.io/corpus/123550.html) | [ẖnmꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4794&db=1) |
| [ϩⲱⲛⲕ](https://coptic-dictionary.org/entry.cgi?tla=C6714) (ID:C6714) | [ḥnk](https://oraec.github.io/corpus/107110.html) | [ḥnk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4145&db=1) |
| [ϩⲛⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6715) (ID:C6715) | [ḥnq.t](https://oraec.github.io/corpus/110300.html) | [ḥq.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4294&db=1) |
| [ϩⲟⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6716) (ID:C6716) | [ḥm-nṯr](https://oraec.github.io/corpus/104940.html) | [ḥm-nṯr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4069&db=1) |
| [ϩⲱⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6718) (ID:C6718) | [ḫnd](https://oraec.github.io/corpus/119430.html) |  |
| [ϩⲉⲛⲉⲉⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6720) (ID:C6720) | [ḥw.t-nṯr](https://oraec.github.io/corpus/99940.html) | [ḥ.t-nṯr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3914&db=1) |
| [ϩⲛⲧⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6722) (ID:C6722) |  | [Hntw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3830&db=1) |
| [ϩⲛⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6723) (ID:C6723) | [ḥn.w](https://oraec.github.io/corpus/106280.html) | [ḥnw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4131&db=1) |
| [ϩⲛⲱⲱϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6728) (ID:C6728) | [ḥr-n-ḥr](https://oraec.github.io/corpus/108010.html) | [ḥnwḥy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4137&db=1) |
| [ϩⲁⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6732) (ID:C6732) | [hp](https://oraec.github.io/corpus/98260.html) | [hpe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3801&db=1) |
| [ϩⲟⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6739) (ID:C6739) | [ḥꜣb](https://oraec.github.io/corpus/103300.html) | [ḥb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4014&db=1) |
| [ϩⲱⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6740) (ID:C6740) | [ḥꜣp](https://oraec.github.io/corpus/101300.html) | [ḥep](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4039&db=1) |
| [ϩⲏⲡⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6743) (ID:C6743) | [ḥꜣp.t](https://oraec.github.io/corpus/101330.html) |  |
| [ϩⲱⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6744) (ID:C6744) | [ꜥb](https://oraec.github.io/corpus/36250.html) | [ꜥb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=914&db=1) |
| [ϩⲁⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6745) (ID:C6745) | [Ḥp](https://oraec.github.io/corpus/104000.html) | [Ḥp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4038&db=1) |
| [ϩⲡⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6748) (ID:C6748) | [ḥpt](https://oraec.github.io/corpus/104240.html) |  |
| [ϩⲟⲡϩⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6750) (ID:C6750) |  | [ḥpḥp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4047&db=1) |
| [ϩⲓⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6756) (ID:C6756) | [ḫr](https://oraec.github.io/corpus/119570.html) | [ẖr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4802&db=1) |
| [ϩⲓⲣϩⲓⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6757) (ID:C6757) |  | [ẖyrẖr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4724&db=1) |
| [ϩⲱⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6759) (ID:C6759) | [ḥri̯](https://oraec.github.io/corpus/108340.html) | [ḥr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4162&db=1) |
| [ϩⲱⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6760) (ID:C6760) | [hrj](https://oraec.github.io/corpus/99010.html) |  |
| [ϩⲱⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6761) (ID:C6761) | [Ḥr.w](https://oraec.github.io/corpus/107500.html) | [Ḥr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4151&db=1) |
| [ϩⲟⲓⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6766) (ID:C6766) |  | [ḥꜥyr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4204&db=1) |
| [ϩⲣⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6768) (ID:C6768) | [ḥr.w](https://oraec.github.io/corpus/108990.html) | [ḥry.w](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4174&db=1) |
| [ϩⲣⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6774) (ID:C6774) | [ẖr.w](https://oraec.github.io/corpus/124420.html) | [ẖr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4799&db=1) |
| [ϩⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6779) (ID:C6779) | [ẖr.t](https://oraec.github.io/corpus/123940.html) | [ẖre.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4834&db=1) |
| [ϩⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6780) (ID:C6780) | [ẖr.t](https://oraec.github.io/corpus/123940.html) | [ẖre.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4834&db=1) |
| [ϩⲣⲓ](https://coptic-dictionary.org/entry.cgi?tla=C6785) (ID:C6785) | [hr.j](https://oraec.github.io/corpus/99020.html) | [hwry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3772&db=1) |
| [ϩⲣⲱ](https://coptic-dictionary.org/entry.cgi?tla=C6787) (ID:C6787) | [ḥry.t](https://oraec.github.io/corpus/108400.html) |  |
| [ϩⲣⲃ](https://coptic-dictionary.org/entry.cgi?tla=C6788) (ID:C6788) | [ḫpr.w](https://oraec.github.io/corpus/116300.html) | [ẖrb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4860&db=1) |
| [ϩⲣⲃ](https://coptic-dictionary.org/entry.cgi?tla=C6790) (ID:C6790) | [ḫrp.w](https://oraec.github.io/corpus/120250.html) |  |
| [ϩⲣⲉⲃ](https://coptic-dictionary.org/entry.cgi?tla=C6791) (ID:C6791) |  | [ḥr-jb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4215&db=1) |
| [ϩⲱⲣⲃ](https://coptic-dictionary.org/entry.cgi?tla=C6792) (ID:C6792) | [ḫrp](https://oraec.github.io/corpus/120150.html) | [ḫrp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4568&db=1) |
| [ϩⲣⲟⲕ](https://coptic-dictionary.org/entry.cgi?tla=C6796) (ID:C6796) | [grḥ](https://oraec.github.io/corpus/167880.html) |  |
| [ϩⲣⲙⲁⲛ](https://coptic-dictionary.org/entry.cgi?tla=C6801) (ID:C6801) | [jnhmn](https://oraec.github.io/corpus/27690.html) | [hrmn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-6983&db=1) |
| [ϩⲱⲣⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6802) (ID:C6802) | [hrp](https://oraec.github.io/corpus/99170.html) | [hrp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3841&db=1) |
| [ϩⲱⲣⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6803) (ID:C6803) | [hrp](https://oraec.github.io/corpus/99170.html) | [hrp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3841&db=1) |
| [ϩⲣⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6807) (ID:C6807) | [hru̯](https://oraec.github.io/corpus/99050.html) | [hre](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3831&db=1) |
| [ϩⲣⲏⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6808) (ID:C6808) | [ḥrr.t](https://oraec.github.io/corpus/109110.html) | [ḥrry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4237&db=1) |
| [ϩⲣⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6812) (ID:C6812) | [gꜣḥ](https://oraec.github.io/corpus/166470.html) |  |
| [ϩⲣⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6815) (ID:C6815) | [ḫrw](https://oraec.github.io/corpus/120010.html) | [ḫrw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4564&db=1) |
| [ϩⲣⲟϣ](https://coptic-dictionary.org/entry.cgi?tla=C6828) (ID:C6828) |  | [ḥrš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4240&db=1) |
| [ϩⲁⲣⲉϩ](https://coptic-dictionary.org/entry.cgi?tla=C6833) (ID:C6833) | [ḥrḥr](https://oraec.github.io/corpus/109180.html) | [ḥrḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4238&db=1) |
| [ϧⲣⲓϫ](https://coptic-dictionary.org/entry.cgi?tla=C6843) (ID:C6843) |  | [ḫrḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4584&db=1) |
| [ϩⲁⲥ](https://coptic-dictionary.org/entry.cgi?tla=C6846) (ID:C6846) | [ḥs](https://oraec.github.io/corpus/109370.html) | [ḥs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4264&db=1) |
| [ϩⲱⲥ](https://coptic-dictionary.org/entry.cgi?tla=C6847) (ID:C6847) | [ḥsi̯](https://oraec.github.io/corpus/109680.html) | [ḥs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7815&db=1) |
| [ϩⲱⲥ](https://coptic-dictionary.org/entry.cgi?tla=C6850) (ID:C6850) | [ḥsꜣ](https://oraec.github.io/corpus/109550.html) | [ḥs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4269&db=1) |
| [ϩⲁⲥⲓⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6851) (ID:C6851) | [ḥz.y](https://oraec.github.io/corpus/109750.html) | [ḥs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4266&db=1) |
| [ϩⲓⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6852) (ID:C6852) | [ẖzi̯](https://oraec.github.io/corpus/124600.html) | [ẖsy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4907&db=1) |
| [ϩⲟⲥⲃ](https://coptic-dictionary.org/entry.cgi?tla=C6862) (ID:C6862) |  | [ḥsbe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4282&db=1) |
| [ϩⲟⲥⲙ](https://coptic-dictionary.org/entry.cgi?tla=C6863) (ID:C6863) | [ḥzmn](https://oraec.github.io/corpus/110020.html) | [ḥsmn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4284&db=1) |
| [ϩⲁⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6864) (ID:C6864) | [ḥḏ](https://oraec.github.io/corpus/112330.html) | [ḥḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4309&db=1) |
| [ϩⲁⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6865) (ID:C6865) | [ḥḏ](https://oraec.github.io/corpus/112300.html) | [ḥḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4374&db=1) |
| [ϩⲁⲉⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6868) (ID:C6868) |  | [ẖyt.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-5187&db=1) |
| [ϩⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6869) (ID:C6869) | [ḥꜣ.tj](https://oraec.github.io/corpus/100400.html) | [ḥꜣty.ṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3947&db=1) |
| [ϩⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6884) (ID:C6884) | [ḫd](https://oraec.github.io/corpus/859285.html) | [ẖdy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4918&db=1) |
| [ϩⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6887) (ID:C6887) | [ḥꜣ.t](https://oraec.github.io/corpus/100310.html) | [ḥꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1087&db=1) |
| [ϩⲓⲉⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6888) (ID:C6888) | [ḥꜣd](https://oraec.github.io/corpus/101770.html) | [hyṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1479&db=1) |
| [ϩⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6889) (ID:C6889) | [hd](https://oraec.github.io/corpus/99620.html) | [hyt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3756&db=1) |
| [ϩⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6890) (ID:C6890) | [ḥꜣd](https://oraec.github.io/corpus/101770.html) |  |
| [ϩⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6891) (ID:C6891) | [ḥtꜣ.w](https://oraec.github.io/corpus/111070.html) | [ḥṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4358&db=1) |
| [ϩⲁⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6895) (ID:C6895) | [ḫdi̯](https://oraec.github.io/corpus/122000.html) | [ẖdy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4919&db=1) |
| [ϩⲓⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6898) (ID:C6898) | [ḫti̯](https://oraec.github.io/corpus/121520.html) | [ẖyṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4727&db=1) |
| [ϩⲟⲓⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6899) (ID:C6899) | [ḥꜣtj](https://oraec.github.io/corpus/101680.html) | [ḥṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4357&db=1) |
| [ϩⲟⲓⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6900) (ID:C6900) | [ḥꜣtj](https://oraec.github.io/corpus/101680.html) | [ḥṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4357&db=1) |
| [ϩⲟⲓⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6901) (ID:C6901) | [ḥṯ.t](https://oraec.github.io/corpus/112040.html) | [ḥyṱy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3970&db=1) |
| [ϩⲟⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6902) (ID:C6902) |  | [ḥṱy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4369&db=1) |
| [ϩⲟⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6909) (ID:C6909) |  | [ḥty.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4326&db=1) |
| [ϩⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6912) (ID:C6912) | [ḫti̯](https://oraec.github.io/corpus/121520.html) | [ẖyṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4727&db=1) |
| [ϩⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6913) (ID:C6913) | [ḥtr](https://oraec.github.io/corpus/111840.html) | [ḥtr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4351&db=1) |
| [ϩⲱϯ](https://coptic-dictionary.org/entry.cgi?tla=C6914) (ID:C6914) |  | [ḥtr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7810&db=1) |
| [ϩⲧⲏ](https://coptic-dictionary.org/entry.cgi?tla=C6917) (ID:C6917) | [ḥt.j](https://oraec.github.io/corpus/111120.html) |  |
| [ϩⲧⲟ](https://coptic-dictionary.org/entry.cgi?tla=C6918) (ID:C6918) | [ḥtr](https://oraec.github.io/corpus/111800.html) | [ḥtr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4348&db=1) |
| [ⲣⲱⲙϩⲧⲟ](https://coptic-dictionary.org/entry.cgi?tla=C6921) (ID:C6921) |  | [rmṯ-ḥtr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1183&db=1) |
| [ϩⲱⲧⲃ](https://coptic-dictionary.org/entry.cgi?tla=C6924) (ID:C6924) | [ẖdb](https://oraec.github.io/corpus/124950.html) | [ẖdb](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4923&db=1) |
| [ϩⲁϯⲗ](https://coptic-dictionary.org/entry.cgi?tla=C6928) (ID:C6928) |  | [ḥtl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4353&db=1) |
| [ϩⲁⲧⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6931) (ID:C6931) | [hdm.w](https://oraec.github.io/corpus/99680.html) | [htmꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3883&db=1) |
| [ϩⲱⲧⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6935) (ID:C6935) | [ḥtp](https://oraec.github.io/corpus/111230.html) | [ḥtp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4332&db=1) |
| [ϩⲧⲟⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6939) (ID:C6939) |  | [ḥtp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4334&db=1) |
| [ϩⲧⲟⲡ](https://coptic-dictionary.org/entry.cgi?tla=C6940) (ID:C6940) | [ḥtp](https://oraec.github.io/corpus/111300.html) |  |
| [ϩⲱⲧⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6943) (ID:C6943) | [ḥtr](https://oraec.github.io/corpus/111860.html) | [ḥtr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4352&db=1) |
| [ϩⲁⲧⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6945) (ID:C6945) | [ḥtr](https://oraec.github.io/corpus/111800.html) | [ḥtr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4346&db=1) |
| [ϩⲉⲧⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6946) (ID:C6946) | [ḥtr](https://oraec.github.io/corpus/111850.html) |  |
| [ϩⲧⲟⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6948) (ID:C6948) |  | [ḥtr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7810&db=1) |
| [ϩⲟⲧⲥ](https://coptic-dictionary.org/entry.cgi?tla=C6951) (ID:C6951) | [hꜣṯs](https://oraec.github.io/corpus/97740.html) |  |
| [ϩϯⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6952) (ID:C6952) |  | [ḥtt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4356&db=1) |
| [ϩⲧⲟⲟⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6953) (ID:C6953) | [dwꜣ.w](https://oraec.github.io/corpus/178000.html) | [dwꜣew](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7140&db=1) |
| [ϩⲁⲑⲱⲣ](https://coptic-dictionary.org/entry.cgi?tla=C6955) (ID:C6955) | [Ḥw.t-Ḥr.w](https://oraec.github.io/corpus/600240.html) |  |
| [ϩⲟⲧϩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6956) (ID:C6956) | [ẖtẖt](https://oraec.github.io/corpus/124920.html) | [ẖtẖte](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4927&db=1) |
| [ϩⲏⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6961) (ID:C6961) | [hꜣw](https://oraec.github.io/corpus/854526.html) | [hy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3733&db=1) |
| [ϩⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6965) (ID:C6965) | [hrw](https://oraec.github.io/corpus/99060.html) | [hrw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3837&db=1) |
| [ⲡⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6968) (ID:C6968) | [pꜣ-hrw](https://oraec.github.io/corpus/58940.html) | [pꜣ-hrw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=1881&db=1) |
| [ϩⲟⲩⲙⲓⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6970) (ID:C6970) |  | [hrw-ms](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-225&db=1) |
| [ϩⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6971) (ID:C6971) | [ḥwꜣ](https://oraec.github.io/corpus/102640.html) | [ḥw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3985&db=1) |
| [ϩⲱⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C6973) (ID:C6973) | [ḥwi̯](https://oraec.github.io/corpus/854530.html) | [ḥwy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3993&db=1) |
| [ϩⲓⲟⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C6977) (ID:C6977) | [ḥwi̯](https://oraec.github.io/corpus/854530.html) | [ḥwy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3994&db=1) |
| [ϩⲟⲩⲟ](https://coptic-dictionary.org/entry.cgi?tla=C6982) (ID:C6982) | [ḥꜣ.w](https://oraec.github.io/corpus/101060.html) | [ḥwe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3984&db=1) |
| [ϩⲟⲩⲣⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C6988) (ID:C6988) | [ḥwrꜥ](https://oraec.github.io/corpus/103170.html) | [ḥwrꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4007&db=1) |
| [ϩⲟⲩⲏⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6991) (ID:C6991) | [hw.tj](https://oraec.github.io/corpus/97980.html) | [hyt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3755&db=1) |
| [ϩⲟⲩⲉⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6992) (ID:C6992) | [ḥꜣ.wtj](https://oraec.github.io/corpus/854603.html) | [ḥꜣṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3936&db=1) |
| [ϩⲟⲩⲉⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6993) (ID:C6993) |  | [ḥꜣ.t.ṱ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-758&db=1) |
| [ϩⲟⲟⲩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C6994) (ID:C6994) | [ꜥḥꜣ.wtj](https://oraec.github.io/corpus/40070.html) | [ḥwṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4012&db=1) |
| [ϩⲟⲟⲩϣ](https://coptic-dictionary.org/entry.cgi?tla=C6999) (ID:C6999) | [hwš](https://oraec.github.io/corpus/600374.html) | [hwš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3776&db=1) |
| [ϩⲟⲩϩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7000) (ID:C7000) |  | [hwh⸮.t?](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3342&db=1) |
| [ϩⲟϥ](https://coptic-dictionary.org/entry.cgi?tla=C7010) (ID:C7010) | [ḥfꜣ.w](https://oraec.github.io/corpus/104390.html) | [ḥf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4049&db=1) |
| [ϩⲟϥ](https://coptic-dictionary.org/entry.cgi?tla=C7011) (ID:C7011) | [ḥfꜣ.w](https://oraec.github.io/corpus/104390.html) | [ḥf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4049&db=1) |
| [ϩⲁϥⲗⲉⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7015) (ID:C7015) | [ḥfnn.t](https://oraec.github.io/corpus/104490.html) | [ḥflelꜥ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4050&db=1) |
| [ϩⲱϥⲧ](https://coptic-dictionary.org/entry.cgi?tla=C7017) (ID:C7017) | [ḥwtf](https://oraec.github.io/corpus/103270.html) | [ḥft](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4052&db=1) |
| [*ϩⲱϥⲧ](https://coptic-dictionary.org/entry.cgi?tla=C7020) (ID:C7020) | [ḥfdi̯](https://oraec.github.io/corpus/104560.html) |  |
| [ϩⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C7021) (ID:C7021) | [ḥḥ](https://oraec.github.io/corpus/109250.html) | [ḥḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4262&db=1) |
| [ϩⲱϩ](https://coptic-dictionary.org/entry.cgi?tla=C7024) (ID:C7024) | [ḫrḫr](https://oraec.github.io/corpus/120420.html) | [ẖẖe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4904&db=1) |
| [ϩⲱϩϥ](https://coptic-dictionary.org/entry.cgi?tla=C7027) (ID:C7027) | [ḫfꜥ](https://oraec.github.io/corpus/116640.html) |  |
| [ϩⲱϫ](https://coptic-dictionary.org/entry.cgi?tla=C7028) (ID:C7028) |  | [ḥꜥḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3983&db=1) |
| [ϩⲁϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7039) (ID:C7039) |  | [ḥqy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4300&db=1) |
| [ϩⲱϭⲃ](https://coptic-dictionary.org/entry.cgi?tla=C7041) (ID:C7041) | [hbq](https://oraec.github.io/corpus/98220.html) | [hbq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3798&db=1) |
| [ϫⲉ-](https://coptic-dictionary.org/entry.cgi?tla=C7055) (ID:C7055) | [r-ḏd](https://oraec.github.io/corpus/859134.html) | [ḏd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7854&db=1) |
| [ϫⲏ](https://coptic-dictionary.org/entry.cgi?tla=C7056) (ID:C7056) | [ḏꜣ](https://oraec.github.io/corpus/181560.html) | [ḏꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-6956&db=1) |
| [ϫⲏ](https://coptic-dictionary.org/entry.cgi?tla=C7057) (ID:C7057) | [ḏꜥꜥ](https://oraec.github.io/corpus/182570.html) | [ḏꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7694&db=1) |
| [ϫⲓ](https://coptic-dictionary.org/entry.cgi?tla=C7058) (ID:C7058) | [ṯꜣi̯](https://oraec.github.io/corpus/174260.html) | [ṯꜣy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7562&db=1) |
| [ϫⲓ](https://coptic-dictionary.org/entry.cgi?tla=C7073) (ID:C7073) | [ṯꜣy](https://oraec.github.io/corpus/174300.html) |  |
| [ϫⲟ](https://coptic-dictionary.org/entry.cgi?tla=C7080) (ID:C7080) | [ḏꜥ](https://oraec.github.io/corpus/182480.html) |  |
| [ϫⲟ](https://coptic-dictionary.org/entry.cgi?tla=C7081) (ID:C7081) |  | [ḏꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7664&db=1) |
| [ϫⲟ](https://coptic-dictionary.org/entry.cgi?tla=C7083) (ID:C7083) | [ḥṯṯ.t](https://oraec.github.io/corpus/112140.html) |  |
| [ϫⲟ](https://coptic-dictionary.org/entry.cgi?tla=C7084) (ID:C7084) | [ḏꜣy.t](https://oraec.github.io/corpus/181870.html) | [ḏyꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7686&db=1) |
| [ϫⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C7087) (ID:C7087) | [ḏꜣ.y](https://oraec.github.io/corpus/181770.html) | [ḏy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7681&db=1) |
| [ϫⲱ](https://coptic-dictionary.org/entry.cgi?tla=C7089) (ID:C7089) | [ḏd](https://oraec.github.io/corpus/185810.html) | [ḏd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7853&db=1) |
| [ϫⲱ](https://coptic-dictionary.org/entry.cgi?tla=C7098) (ID:C7098) |  | [ḏd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7856&db=1) |
| [ϫⲃⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C7106) (ID:C7106) | [ḏnb](https://oraec.github.io/corpus/184240.html) |  |
| [ϫⲱⲕ](https://coptic-dictionary.org/entry.cgi?tla=C7119) (ID:C7119) |  | [ḏq](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7829&db=1) |
| [ϫⲱⲕⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7124) (ID:C7124) |  | [ḏqꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7831&db=1) |
| [ϫⲱⲕⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7131) (ID:C7131) |  | [ḏqm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7832&db=1) |
| [ϫⲟⲕϫⲕ](https://coptic-dictionary.org/entry.cgi?tla=C7145) (ID:C7145) | [tktk](https://oraec.github.io/corpus/173770.html) |  |
| [ϫⲁⲗ](https://coptic-dictionary.org/entry.cgi?tla=C7148) (ID:C7148) | [ḏnr](https://oraec.github.io/corpus/184350.html) |  |
| [ϫⲟⲗ](https://coptic-dictionary.org/entry.cgi?tla=C7150) (ID:C7150) | [wḏn.w](https://oraec.github.io/corpus/52710.html) |  |
| [ϫⲱⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7160) (ID:C7160) | [ḏꜥr](https://oraec.github.io/corpus/854589.html) | [ḏlꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7802&db=1) |
| [ϫⲱⲱⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7164) (ID:C7164) | [ṯnr](https://oraec.github.io/corpus/550245.html) | [ḏr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-919&db=1) |
| [ϫⲗⲁ](https://coptic-dictionary.org/entry.cgi?tla=C7167) (ID:C7167) |  | [ḏlꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7804&db=1) |
| [ϫⲗⲱⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7189) (ID:C7189) | [ṯnm](https://oraec.github.io/corpus/175960.html) |  |
| [ϫⲟⲗϩ](https://coptic-dictionary.org/entry.cgi?tla=C7195) (ID:C7195) | [ṯrḥ](https://oraec.github.io/corpus/176410.html) | [ḏlḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7811&db=1) |
| [ϫⲱⲗϩ](https://coptic-dictionary.org/entry.cgi?tla=C7198) (ID:C7198) |  | [ḏlḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7810&db=1) |
| [ϫⲟⲗϫⲗ](https://coptic-dictionary.org/entry.cgi?tla=C7211) (ID:C7211) |  | [ḏlḏyl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7819&db=1) |
| [ϫⲟⲗϫⲗ](https://coptic-dictionary.org/entry.cgi?tla=C7212) (ID:C7212) | [ḏrḏr](https://oraec.github.io/corpus/185170.html) | [ḏlḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7816&db=1) |
| [ϫⲟⲗϫⲗ](https://coptic-dictionary.org/entry.cgi?tla=C7213) (ID:C7213) |  | [ḏlḏl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7817&db=1) |
| [ϫⲱⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7215) (ID:C7215) | [ḏꜣm](https://oraec.github.io/corpus/182160.html) | [ḏm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7740&db=1) |
| [ϫⲱⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7216) (ID:C7216) | [ḏꜣm](https://oraec.github.io/corpus/182150.html) |  |
| [ϫⲁⲙⲏ](https://coptic-dictionary.org/entry.cgi?tla=C7218) (ID:C7218) |  | [ḏme](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3641&db=1) |
| [ϫⲱⲱⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7219) (ID:C7219) | [ḏmꜥ](https://oraec.github.io/corpus/184040.html) | [ḏmꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7748&db=1) |
| [ϫⲱⲱⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7220) (ID:C7220) | [ḏmꜥ](https://oraec.github.io/corpus/184040.html) | [ḏmꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7748&db=1) |
| [ϫⲙⲡⲉϩ](https://coptic-dictionary.org/entry.cgi?tla=C7225) (ID:C7225) | [ḏpḥ](https://oraec.github.io/corpus/183730.html) | [ḏpḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7730&db=1) |
| [ϫⲓⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C7232) (ID:C7232) | [n-ṯꜣ](https://oraec.github.io/corpus/600481.html) | [n-ṯꜣy-n](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2913&db=1) |
| [ϫⲓⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C7233) (ID:C7233) | [n-ṯꜣ](https://oraec.github.io/corpus/600481.html) | [n-ṯꜣy-n](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2913&db=1) |
| [ϫⲁⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7236) (ID:C7236) | [ḏnn.t](https://oraec.github.io/corpus/184340.html) |  |
| [ϫⲁⲛⲟ](https://coptic-dictionary.org/entry.cgi?tla=C7238) (ID:C7238) |  | [ḏny.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-6978&db=1) |
| [ϫⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7245) (ID:C7245) | [ḏn.w](https://oraec.github.io/corpus/184120.html) |  |
| [ϫⲛⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C7246) (ID:C7246) | [sṯni̯](https://oraec.github.io/corpus/854556.html) | [sḏny](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=5794&db=1) |
| [ϫⲱⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C7251) (ID:C7251) |  | [ḏnt](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7768&db=1) |
| [ϫⲛⲁⲩ](https://coptic-dictionary.org/entry.cgi?tla=C7259) (ID:C7259) | [ṯnj](https://oraec.github.io/corpus/175780.html) |  |
| [ϫⲛⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C7265) (ID:C7265) | [ḏn.w](https://oraec.github.io/corpus/184220.html) | [ḏnw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7759&db=1) |
| [ϫⲱⲛϥ](https://coptic-dictionary.org/entry.cgi?tla=C7267) (ID:C7267) | [ṯnf](https://oraec.github.io/corpus/175920.html) | [ḏnf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7762&db=1) |
| [ϫⲛⲟϥ](https://coptic-dictionary.org/entry.cgi?tla=C7270) (ID:C7270) | [ṯnf](https://oraec.github.io/corpus/175900.html) | [ḏnf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7716&db=1) |
| [ϫⲛⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C7271) (ID:C7271) | [ḏnḥ](https://oraec.github.io/corpus/184390.html) | [ḏnḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7767&db=1) |
| [ϫⲟⲡ](https://coptic-dictionary.org/entry.cgi?tla=C7288) (ID:C7288) | [ṯꜣb](https://oraec.github.io/corpus/174560.html) | [ḏpe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7729&db=1) |
| [ϫⲉⲡⲓ](https://coptic-dictionary.org/entry.cgi?tla=C7292) (ID:C7292) |  | [pk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=2162&db=1) |
| [ϫⲏⲣ](https://coptic-dictionary.org/entry.cgi?tla=C7306) (ID:C7306) | [ḏrꜥ](https://oraec.github.io/corpus/184960.html) | [ḏrꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7783&db=1) |
| [ⲁⲛϫⲓⲣ](https://coptic-dictionary.org/entry.cgi?tla=C7313) (ID:C7313) |  | [ꜣnḏyr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=132&db=1) |
| [ϫⲱⲣ](https://coptic-dictionary.org/entry.cgi?tla=C7316) (ID:C7316) | [ḏꜥr](https://oraec.github.io/corpus/854589.html) | [ḏlꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7802&db=1) |
| [ϫⲉⲣⲟ](https://coptic-dictionary.org/entry.cgi?tla=C7321) (ID:C7321) |  | [ṯꜣy-rꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3974&db=1) |
| [ϫⲏⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7324) (ID:C7324) |  | [ḏry.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7782&db=1) |
| [ϫⲓⲉⲓⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7327) (ID:C7327) | [ḏꜣr.t](https://oraec.github.io/corpus/182260.html) | [ṯꜣy-jr.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3081&db=1) |
| [ϫⲱⲱⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7328) (ID:C7328) | [ḏrꜥ](https://oraec.github.io/corpus/184960.html) | [ḏrꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7783&db=1) |
| [ϫⲣⲟ](https://coptic-dictionary.org/entry.cgi?tla=C7332) (ID:C7332) | [ḏrj](https://oraec.github.io/corpus/184860.html) | [ḏr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7775&db=1) |
| [ϫⲱⲱⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7341) (ID:C7341) | [ṯnr](https://oraec.github.io/corpus/550245.html) | [ḏr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-919&db=1) |
| [ϫⲱⲣⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7352) (ID:C7352) | [ṯrm](https://oraec.github.io/corpus/176380.html) | [ḏrm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7789&db=1) |
| [ϫⲱⲣⲡ](https://coptic-dictionary.org/entry.cgi?tla=C7357) (ID:C7357) | [ṯrp](https://oraec.github.io/corpus/176360.html) | [ḏrp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7786&db=1) |
| [ϫⲟⲉⲓⲥ](https://coptic-dictionary.org/entry.cgi?tla=C7376) (ID:C7376) | [ṯꜣz.w](https://oraec.github.io/corpus/177110.html) | [ṯsyꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7649&db=1) |
| [ϫⲟⲉⲓⲥ](https://coptic-dictionary.org/entry.cgi?tla=C7377) (ID:C7377) | [ṯꜣz.w](https://oraec.github.io/corpus/177110.html) | [ṯsyꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7649&db=1) |
| [ϫⲱⲥ](https://coptic-dictionary.org/entry.cgi?tla=C7381) (ID:C7381) | [ṯꜣz](https://oraec.github.io/corpus/176800.html) | [ṯs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7648&db=1) |
| [ϫⲓⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7382) (ID:C7382) | [ṯzi̯](https://oraec.github.io/corpus/854581.html) | [ṯs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7652&db=1) |
| [ϫⲓⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7387) (ID:C7387) |  | [ṯsy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7658&db=1) |
| [ϫⲓⲥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7394) (ID:C7394) | [ṯꜣz.t](https://oraec.github.io/corpus/176930.html) | [ṯse.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7656&db=1) |
| [ϫⲁⲥϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7395) (ID:C7395) |  | [ḏsfꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7828&db=1) |
| [ϫⲟⲉⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C7400) (ID:C7400) | [ḏt](https://oraec.github.io/corpus/185770.html) | [ḏyṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7691&db=1) |
| [ϫⲟⲉⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C7401) (ID:C7401) | [ḏt](https://oraec.github.io/corpus/185770.html) | [ḏyṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7691&db=1) |
| [ϫⲟⲉⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C7402) (ID:C7402) | [ḏt](https://oraec.github.io/corpus/185770.html) | [ḏyṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7691&db=1) |
| [ϫⲟⲉⲓⲧ](https://coptic-dictionary.org/entry.cgi?tla=C7403) (ID:C7403) | [ḏt](https://oraec.github.io/corpus/185770.html) | [ḏyṱ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7691&db=1) |
| [ϫⲁⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7408) (ID:C7408) | [ḏdꜣ](https://oraec.github.io/corpus/186090.html) |  |
| [ϫⲱⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7410) (ID:C7410) | [ḏꜣd](https://oraec.github.io/corpus/182290.html) |  |
| [ϫⲁⲧⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7416) (ID:C7416) | [ḏdm.t](https://oraec.github.io/corpus/186290.html) | [ḏtm.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3268&db=1) |
| [ϫⲁⲧϥⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7417) (ID:C7417) | [ḏdf.t](https://oraec.github.io/corpus/186250.html) | [ḏdfe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-108&db=1) |
| [ϫⲧⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C7419) (ID:C7419) |  | [ḏdḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7904&db=1) |
| [ϫⲓⲟⲩⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7425) (ID:C7425) | [ṯꜣu̯](https://oraec.github.io/corpus/174470.html) | [ḏwy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7718&db=1) |
| [ϫⲁⲩⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7433) (ID:C7433) | [ṯni̯](https://oraec.github.io/corpus/175750.html) | [tne](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7307&db=1) |
| [ϫⲟⲟⲩϥ](https://coptic-dictionary.org/entry.cgi?tla=C7440) (ID:C7440) | [ṯwfj](https://oraec.github.io/corpus/174970.html) | [ḏwf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7719&db=1) |
| [ϫⲟⲩϥ](https://coptic-dictionary.org/entry.cgi?tla=C7455) (ID:C7455) | [ḏꜣf](https://oraec.github.io/corpus/182120.html) | [ḏf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7734&db=1) |
| [ⲛϫⲟϥⲧⲛ](https://coptic-dictionary.org/entry.cgi?tla=C7465) (ID:C7465) | [ṯftn](https://oraec.github.io/corpus/855232.html) | [ḏftn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7738&db=1) |
| [ϫⲟϥϫϥ](https://coptic-dictionary.org/entry.cgi?tla=C7466) (ID:C7466) |  | [ḏfḏf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7739&db=1) |
| [ϫⳉⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C7468) (ID:C7468) |  | [ḫꜥḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-4656&db=1) |
| [ϫⲓϩ](https://coptic-dictionary.org/entry.cgi?tla=C7471) (ID:C7471) |  | [ḏꜣk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7675&db=1) |
| [ϫⲱϩ](https://coptic-dictionary.org/entry.cgi?tla=C7472) (ID:C7472) | [ṯḥj](https://oraec.github.io/corpus/176510.html) | [ḏḥe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7822&db=1) |
| [ϫⲱϩⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7482) (ID:C7482) |  | [ḏẖm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7827&db=1) |
| [ϫⲁϫ](https://coptic-dictionary.org/entry.cgi?tla=C7493) (ID:C7493) | [ṯṯ](https://oraec.github.io/corpus/177580.html) |  |
| [ϫⲱϫ](https://coptic-dictionary.org/entry.cgi?tla=C7497) (ID:C7497) | [ḏꜣḏꜣ](https://oraec.github.io/corpus/182330.html) | [ḏꜣḏꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7677&db=1) |
| [ⲉϫⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C7504) (ID:C7504) |  | [r-ḏꜣḏꜣ-n](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=3407&db=1) |
| [ϩⲁϫⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C7506) (ID:C7506) |  | [ẖr-ḏꜣḏꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4821&db=1) |
| [ϩⲓϫⲛ-](https://coptic-dictionary.org/entry.cgi?tla=C7508) (ID:C7508) | [ḥr-ḏꜣḏꜣ](https://oraec.github.io/corpus/600345.html) | [ḥr-ḏꜣḏꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=4203&db=1) |
| [ϫⲁϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7521) (ID:C7521) | [ḏrḏr](https://oraec.github.io/corpus/650046.html) | [ḏḏy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7866&db=1) |
| [ϫⲁϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7522) (ID:C7522) | [ḏrḏr](https://oraec.github.io/corpus/650046.html) | [ḏḏy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7866&db=1) |
| [ϫⲓϫⲱⲓ](https://coptic-dictionary.org/entry.cgi?tla=C7530) (ID:C7530) |  | [ṯꜣy-ḏꜣḏꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7635&db=1) |
| [ϫⲁϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7534) (ID:C7534) | [gṯ](https://oraec.github.io/corpus/855234.html) |  |
| [ϫⲱϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7540) (ID:C7540) |  | [ṯk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-3206&db=1) |
| [ϭⲁ](https://coptic-dictionary.org/entry.cgi?tla=C7548) (ID:C7548) | [gꜣi̯](https://oraec.github.io/corpus/166130.html) | [gꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6679&db=1) |
| [ϭⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C7549) (ID:C7549) | [gꜣy](https://oraec.github.io/corpus/166140.html) | [gy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6702&db=1) |
| [ϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7550) (ID:C7550) | [gr.t](https://oraec.github.io/corpus/167790.html) | [gꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6681&db=1) |
| [ϭⲓ](https://coptic-dictionary.org/entry.cgi?tla=C7552) (ID:C7552) | [qj](https://oraec.github.io/corpus/159670.html) | [gy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6698&db=1) |
| [ϭⲓ](https://coptic-dictionary.org/entry.cgi?tla=C7553) (ID:C7553) | [Gꜣy](https://oraec.github.io/corpus/166170.html) |  |
| [ϭⲱ](https://coptic-dictionary.org/entry.cgi?tla=C7555) (ID:C7555) | [gr](https://oraec.github.io/corpus/167750.html) | [gr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6819&db=1) |
| [ϭⲱⲱⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7560) (ID:C7560) | [gꜣb.t](https://oraec.github.io/corpus/166380.html) | [gbꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6767&db=1) |
| [ϭⲃⲓⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7564) (ID:C7564) | [gbi̯](https://oraec.github.io/corpus/166950.html) | [gby](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6762&db=1) |
| [ϭⲃⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C7565) (ID:C7565) | [gbꜣ](https://oraec.github.io/corpus/166900.html) | [gby](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-627&db=1) |
| [ϭⲃⲃⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7566) (ID:C7566) | [gbi̯](https://oraec.github.io/corpus/166950.html) | [gby](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6762&db=1) |
| [ϭⲱⲃ](https://coptic-dictionary.org/entry.cgi?tla=C7571) (ID:C7571) |  | [gbe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-915&db=1) |
| [ϭⲃϭⲱⲃ⸗](https://coptic-dictionary.org/entry.cgi?tla=C7580) (ID:C7580) | [gbgb](https://oraec.github.io/corpus/167050.html) |  |
| [ϭⲗ](https://coptic-dictionary.org/entry.cgi?tla=C7583) (ID:C7583) | [qrꜥ.w](https://oraec.github.io/corpus/161670.html) | [glꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6891&db=1) |
| [ϭⲟⲗ](https://coptic-dictionary.org/entry.cgi?tla=C7588) (ID:C7588) | [grg](https://oraec.github.io/corpus/168040.html) | [glk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6907&db=1) |
| [ϭⲱⲗ](https://coptic-dictionary.org/entry.cgi?tla=C7597) (ID:C7597) | [ḏꜥr](https://oraec.github.io/corpus/854589.html) | [ḏlꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7802&db=1) |
| [ϭⲱⲗ](https://coptic-dictionary.org/entry.cgi?tla=C7599) (ID:C7599) |  | [glꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6892&db=1) |
| [ϭⲁⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7605) (ID:C7605) |  | [gle](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6880&db=1) |
| [ϭⲁⲗⲏ](https://coptic-dictionary.org/entry.cgi?tla=C7606) (ID:C7606) |  | [gle](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6880&db=1) |
| [ϭⲁⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7607) (ID:C7607) |  | [gle](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6880&db=1) |
| [ϭⲁⲗⲏ](https://coptic-dictionary.org/entry.cgi?tla=C7608) (ID:C7608) |  | [gle](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6880&db=1) |
| [ϭⲟⲓⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7613) (ID:C7613) | [qꜣri̯](https://oraec.github.io/corpus/850645.html) | [gyly](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6709&db=1) |
| [ϭⲱⲱⲗⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7623) (ID:C7623) | [qꜣri̯](https://oraec.github.io/corpus/850645.html) | [glw](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6895&db=1) |
| [ϭⲗⲏ](https://coptic-dictionary.org/entry.cgi?tla=C7636) (ID:C7636) | [ḏꜣr.t](https://oraec.github.io/corpus/182270.html) | [ḏry](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7781&db=1) |
| [ϭⲗⲏ](https://coptic-dictionary.org/entry.cgi?tla=C7637) (ID:C7637) | [qni̯](https://oraec.github.io/corpus/854565.html) | [qne](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6355&db=1) |
| [ϭⲗⲟ](https://coptic-dictionary.org/entry.cgi?tla=C7642) (ID:C7642) | [ḏr](https://oraec.github.io/corpus/184570.html) |  |
| [ϭⲗⲟⲓ](https://coptic-dictionary.org/entry.cgi?tla=C7645) (ID:C7645) |  | [klꜥy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6631&db=1) |
| [ϭⲉⲗⲃⲉⲥⲓ](https://coptic-dictionary.org/entry.cgi?tla=C7651) (ID:C7651) |  | [krbsy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-754&db=1) |
| [ϭⲗⲃⲟⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C7653) (ID:C7653) | [gb.t](https://oraec.github.io/corpus/166880.html) |  |
| [ϭⲗⲓⲗ](https://coptic-dictionary.org/entry.cgi?tla=C7658) (ID:C7658) | [qrr](https://oraec.github.io/corpus/161820.html) | [gll](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6902&db=1) |
| [ϭⲗⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7660) (ID:C7660) |  | [glme](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6899&db=1) |
| [ϭⲗⲙⲁⲓ](https://coptic-dictionary.org/entry.cgi?tla=C7662) (ID:C7662) |  | [qlby](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6424&db=1) |
| [ϭⲗⲟⲙⲗⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7663) (ID:C7663) |  | [glmlm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6900&db=1) |
| [ϭⲱⲗⲡ](https://coptic-dictionary.org/entry.cgi?tla=C7668) (ID:C7668) | [krp](https://oraec.github.io/corpus/852966.html) | [glp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6897&db=1) |
| [ϭⲗⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7682) (ID:C7682) | [qrt](https://oraec.github.io/corpus/162030.html) | [glṱ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6915&db=1) |
| [ϭⲁⲗⲓⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7683) (ID:C7683) |  | [glyṱꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6890&db=1) |
| [ϭⲁⲗⲁϣⲓⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7688) (ID:C7688) | [kr-šrj](https://oraec.github.io/corpus/600321.html) | [gl-šr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6884&db=1) |
| [ϭⲁⲗⲁϩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C7690) (ID:C7690) | [qrḥ.t](https://oraec.github.io/corpus/161890.html) |  |
| [ϭⲱⲗϫ](https://coptic-dictionary.org/entry.cgi?tla=C7692) (ID:C7692) |  | [glḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6916&db=1) |
| [ϭⲗⲟϭ](https://coptic-dictionary.org/entry.cgi?tla=C7696) (ID:C7696) |  | [glge](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6910&db=1) |
| [ϭⲗⲟϭ](https://coptic-dictionary.org/entry.cgi?tla=C7697) (ID:C7697) | [dnrg](https://oraec.github.io/corpus/600464.html) | [glg](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6908&db=1) |
| [ϭⲟⲗϭⲗ](https://coptic-dictionary.org/entry.cgi?tla=C7703) (ID:C7703) |  | [ḏlḏl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7817&db=1) |
| [ϭⲁⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7705) (ID:C7705) |  | [gm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6789&db=1) |
| [ϭⲟⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7706) (ID:C7706) |  | [gmꜣe.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6787&db=1) |
| [ϭⲟⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7723) (ID:C7723) |  | [qmy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6339&db=1) |
| [ϭⲱⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7724) (ID:C7724) | [kꜣn.w](https://oraec.github.io/corpus/163590.html) | [kꜣm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6520&db=1) |
| [ϭⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7725) (ID:C7725) | [kꜣn.w](https://oraec.github.io/corpus/163600.html) | [kꜣmy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6522&db=1) |
| [ϭⲁⲓⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7729) (ID:C7729) | [gm.t](https://oraec.github.io/corpus/167160.html) | [kymy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-1307&db=1) |
| [ϭⲱⲱⲙⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7732) (ID:C7732) |  | [gmꜥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6794&db=1) |
| [ϭⲁⲙⲟⲩⲗ](https://coptic-dictionary.org/entry.cgi?tla=C7737) (ID:C7737) |  | [gmwl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6797&db=1) |
| [ⲙⲁⲛϭⲁⲙⲟⲩⲗ](https://coptic-dictionary.org/entry.cgi?tla=C7739) (ID:C7739) |  | [mny-gmwl](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-6417&db=1) |
| [ϭⲱⲙϩ](https://coptic-dictionary.org/entry.cgi?tla=C7740) (ID:C7740) | [gmḥ](https://oraec.github.io/corpus/167270.html) |  |
| [ϭⲟⲙϭⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7741) (ID:C7741) |  | [kmkm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6585&db=1) |
| [ϭⲓⲛⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7750) (ID:C7750) | [gmi̯](https://oraec.github.io/corpus/167210.html) | [gm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6784&db=1) |
| [ϭⲛⲟ](https://coptic-dictionary.org/entry.cgi?tla=C7761) (ID:C7761) | [qni̯](https://oraec.github.io/corpus/854565.html) | [qne](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6355&db=1) |
| [ϭⲱⲛⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7762) (ID:C7762) | [kꜣmn](https://oraec.github.io/corpus/163570.html) | [gnme](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6809&db=1) |
| [ϭⲓⲛⲙⲟⲩⲧ](https://coptic-dictionary.org/entry.cgi?tla=C7763) (ID:C7763) | [knm.tj](https://oraec.github.io/corpus/164870.html) |  |
| [ϭⲛⲟⲛ](https://coptic-dictionary.org/entry.cgi?tla=C7765) (ID:C7765) | [gnn](https://oraec.github.io/corpus/167540.html) | [gnn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6811&db=1) |
| [ϭⲟⲛ](https://coptic-dictionary.org/entry.cgi?tla=C7767) (ID:C7767) | [gnn](https://oraec.github.io/corpus/600572.html) | [gn](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6802&db=1) |
| [ϭⲓⲛⲏⲣⲁ](https://coptic-dictionary.org/entry.cgi?tla=C7774) (ID:C7774) | [knnr](https://oraec.github.io/corpus/164760.html) |  |
| [ϭⲟⲛⲥ](https://coptic-dictionary.org/entry.cgi?tla=C7775) (ID:C7775) | [gns](https://oraec.github.io/corpus/167670.html) | [gnse](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6816&db=1) |
| [ϭⲱⲛⲧ](https://coptic-dictionary.org/entry.cgi?tla=C7787) (ID:C7787) | [qnd](https://oraec.github.io/corpus/161520.html) | [qnd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6378&db=1) |
| [ϭⲛⲁⲧ](https://coptic-dictionary.org/entry.cgi?tla=C7795) (ID:C7795) | [qnd](https://oraec.github.io/corpus/161520.html) | [qnd](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6378&db=1) |
| [ϭⲓⲛⲟⲩⲏⲗ](https://coptic-dictionary.org/entry.cgi?tla=C7803) (ID:C7803) | [kbn.t](https://oraec.github.io/corpus/163990.html) |  |
| [ϭⲛⲟⲩϥ](https://coptic-dictionary.org/entry.cgi?tla=C7804) (ID:C7804) | [ṯnf](https://oraec.github.io/corpus/175900.html) | [ḏnf](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7763&db=1) |
| [ϭⲁⲛⲁϩ](https://coptic-dictionary.org/entry.cgi?tla=C7806) (ID:C7806) | [gꜣḥ](https://oraec.github.io/corpus/166480.html) |  |
| [ϭⲓⲛϭⲗⲱ](https://coptic-dictionary.org/entry.cgi?tla=C7812) (ID:C7812) |  | [gnglꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6818&db=1) |
| [ϭⲛϭⲛ](https://coptic-dictionary.org/entry.cgi?tla=C7813) (ID:C7813) | [qnqn](https://oraec.github.io/corpus/161450.html) | [qnqne](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6376&db=1) |
| [ϭⲓⲛϭⲓⲛ](https://coptic-dictionary.org/entry.cgi?tla=C7816) (ID:C7816) | [gngn.t](https://oraec.github.io/corpus/167700.html) |  |
| [ϭⲓⲛϭⲱⲣ](https://coptic-dictionary.org/entry.cgi?tla=C7817) (ID:C7817) |  | [krkr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6622&db=1) |
| [ϭⲛϭⲉϩ](https://coptic-dictionary.org/entry.cgi?tla=C7818) (ID:C7818) |  | [gnḥḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6815&db=1) |
| [ϭⲟⲡ](https://coptic-dictionary.org/entry.cgi?tla=C7819) (ID:C7819) |  | [gpe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6775&db=1) |
| [ϭⲏⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7827) (ID:C7827) |  | [gp.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6776&db=1) |
| [ϭⲱⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7830) (ID:C7830) |  | [kp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6563&db=1) |
| [ϭⲁⲡⲓϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7846) (ID:C7846) |  | [kpḏ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6571&db=1) |
| [ϭⲁⲡⲓϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7847) (ID:C7847) |  | [kpḏ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6571&db=1) |
| [ϭⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7853) (ID:C7853) | [gry](https://oraec.github.io/corpus/167810.html) |  |
| [ϭⲣⲱ](https://coptic-dictionary.org/entry.cgi?tla=C7857) (ID:C7857) | [nqw.t](https://oraec.github.io/corpus/89070.html) |  |
| [ϭⲱⲣⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7861) (ID:C7861) | [grm](https://oraec.github.io/corpus/167860.html) |  |
| [ϭⲣⲟⲟⲙⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7863) (ID:C7863) | [gr-n-p.t](https://oraec.github.io/corpus/167820.html) | [grmp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6857&db=1) |
| [ϭⲣⲟⲟⲙⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7864) (ID:C7864) | [gr-n-p.t](https://oraec.github.io/corpus/167820.html) | [grmp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6857&db=1) |
| [ϭⲣⲏⲡⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7870) (ID:C7870) |  | [grpꜣ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6852&db=1) |
| [ϭⲁⲣⲁⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7876) (ID:C7876) | [grt](https://oraec.github.io/corpus/863678.html) |  |
| [ϭⲟⲣⲧⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7877) (ID:C7877) | [qrḏn](https://oraec.github.io/corpus/162060.html) | [grṱy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6878&db=1) |
| [ϭⲟⲣϥ⸗](https://coptic-dictionary.org/entry.cgi?tla=C7879) (ID:C7879) | [krp](https://oraec.github.io/corpus/165060.html) | [grp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-7578&db=1) |
| [ϭⲱⲣϩ](https://coptic-dictionary.org/entry.cgi?tla=C7880) (ID:C7880) | [grḥ](https://oraec.github.io/corpus/167920.html) | [grḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6863&db=1) |
| [ϭⲣⲱϩ](https://coptic-dictionary.org/entry.cgi?tla=C7883) (ID:C7883) | [grḥ](https://oraec.github.io/corpus/167880.html) | [ḏrḥ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7791&db=1) |
| [ϭⲟⲣϫ](https://coptic-dictionary.org/entry.cgi?tla=C7888) (ID:C7888) |  | [krky](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6621&db=1) |
| [ϫⲉⲣϫⲓ](https://coptic-dictionary.org/entry.cgi?tla=C7889) (ID:C7889) |  | [krky](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6621&db=1) |
| [ϫⲉⲣϫⲓ](https://coptic-dictionary.org/entry.cgi?tla=C7890) (ID:C7890) |  | [krky](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6621&db=1) |
| [ϭⲱⲣϭ](https://coptic-dictionary.org/entry.cgi?tla=C7893) (ID:C7893) | [grg](https://oraec.github.io/corpus/854571.html) | [grg](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6867&db=1) |
| [ϭⲉⲣⲏϭ](https://coptic-dictionary.org/entry.cgi?tla=C7898) (ID:C7898) | [grg](https://oraec.github.io/corpus/167990.html) | [grg](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6868&db=1) |
| [ϭⲱⲣϭ](https://coptic-dictionary.org/entry.cgi?tla=C7900) (ID:C7900) | [grg](https://oraec.github.io/corpus/854571.html) | [grg](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6869&db=1) |
| [ϭⲱⲣϭ](https://coptic-dictionary.org/entry.cgi?tla=C7903) (ID:C7903) | [grg](https://oraec.github.io/corpus/854571.html) | [grg](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6869&db=1) |
| [ϭⲣⲏϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7913) (ID:C7913) |  | [grg.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6873&db=1) |
| [ϭⲟⲥ](https://coptic-dictionary.org/entry.cgi?tla=C7917) (ID:C7917) | [gs](https://oraec.github.io/corpus/854572.html) | [gs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6922&db=1) |
| [ϭⲟⲥⲙ](https://coptic-dictionary.org/entry.cgi?tla=C7922) (ID:C7922) |  | [gsm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6935&db=1) |
| [ϭⲟⲥⲧ](https://coptic-dictionary.org/entry.cgi?tla=C7925) (ID:C7925) | [gstj](https://oraec.github.io/corpus/168670.html) | [gsṱe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6942&db=1) |
| [ϭⲟⲥϭⲥ](https://coptic-dictionary.org/entry.cgi?tla=C7926) (ID:C7926) | [ksks](https://oraec.github.io/corpus/165520.html) | [gsgs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6939&db=1) |
| [ϭⲟⲥϭⲥ](https://coptic-dictionary.org/entry.cgi?tla=C7927) (ID:C7927) | [ksks](https://oraec.github.io/corpus/165520.html) | [gsgs](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6939&db=1) |
| [ϭⲟⲧ](https://coptic-dictionary.org/entry.cgi?tla=C7929) (ID:C7929) | [qd](https://oraec.github.io/corpus/162430.html) | [qdy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6487&db=1) |
| [ϭⲱⲧ](https://coptic-dictionary.org/entry.cgi?tla=C7933) (ID:C7933) |  | [gt.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6950&db=1) |
| [ϭⲱⲧⲡ](https://coptic-dictionary.org/entry.cgi?tla=C7936) (ID:C7936) |  | [gtp](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6957&db=1) |
| [ϭⲱⲧϩ](https://coptic-dictionary.org/entry.cgi?tla=C7949) (ID:C7949) |  | [ḏthe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7845&db=1) |
| [ϭⲱⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C7956) (ID:C7956) | [gꜣu̯](https://oraec.github.io/corpus/166210.html) | [gwꜣ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6742&db=1) |
| [ϭⲱⲟⲩ](https://coptic-dictionary.org/entry.cgi?tla=C7959) (ID:C7959) | [gwꜣ](https://oraec.github.io/corpus/166730.html) |  |
| [ϭⲟⲟⲩⲣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7973) (ID:C7973) | [qwr](https://oraec.github.io/corpus/159970.html) | [gwr](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6749&db=1) |
| [ϭⲱⲟⲩϭ](https://coptic-dictionary.org/entry.cgi?tla=C7974) (ID:C7974) | [gwš](https://oraec.github.io/corpus/166820.html) | [gwš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=-550&db=1) |
| [ϭⲱϣ](https://coptic-dictionary.org/entry.cgi?tla=C7976) (ID:C7976) |  | [gš](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6944&db=1) |
| [ϭⲏϣⲉ](https://coptic-dictionary.org/entry.cgi?tla=C7980) (ID:C7980) | [gš](https://oraec.github.io/corpus/168690.html) |  |
| [ϭⲱϣⲧ](https://coptic-dictionary.org/entry.cgi?tla=C7982) (ID:C7982) |  | [gšpe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6946&db=1) |
| [ϭϩⲟⲥ](https://coptic-dictionary.org/entry.cgi?tla=C7994) (ID:C7994) | [gḥs](https://oraec.github.io/corpus/168210.html) | [gḥsy.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6920&db=1) |
| [ϭⲓϫ](https://coptic-dictionary.org/entry.cgi?tla=C7995) (ID:C7995) |  | [gyḏ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6713&db=1) |
| [ϭⲟⲩϫ](https://coptic-dictionary.org/entry.cgi?tla=C8004) (ID:C8004) | [qḏ](https://oraec.github.io/corpus/162690.html) | [gḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6966&db=1) |
| [ϭⲁϫⲉ](https://coptic-dictionary.org/entry.cgi?tla=C8005) (ID:C8005) |  | [gḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6965&db=1) |
| [ϭⲟϫⲓ](https://coptic-dictionary.org/entry.cgi?tla=C8006) (ID:C8006) |  | [ḏḏy](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=7868&db=1) |
| [ϭⲁϫⲙⲏ](https://coptic-dictionary.org/entry.cgi?tla=C8025) (ID:C8025) |  | [gḏm](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6970&db=1) |
| [ϭⲁϫⲓϥ](https://coptic-dictionary.org/entry.cgi?tla=C8027) (ID:C8027) |  | [qpqpe](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6323&db=1) |
| [ϭⲟϫϭϫ](https://coptic-dictionary.org/entry.cgi?tla=C8029) (ID:C8029) | [ktkt](https://oraec.github.io/corpus/165810.html) | [kḏkḏ](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6670&db=1) |
| [ϭⲱϭ](https://coptic-dictionary.org/entry.cgi?tla=C8032) (ID:C8032) |  | [kk](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6660&db=1) |
| [ϭⲁⲁϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C8035) (ID:C8035) | [ꜥkk](https://oraec.github.io/corpus/41610.html) | [kꜥkꜥ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6539&db=1) |
| [ϭⲁⲁϭⲉ](https://coptic-dictionary.org/entry.cgi?tla=C8036) (ID:C8036) | [ꜥkk](https://oraec.github.io/corpus/41610.html) | [kꜥkꜥ.t](https://aaew.bbaw.de/tla/servlet/GetWcnDetails?&wn=6539&db=1) |

As you can see, this list is based on the Coptic words. We have also sorted the list according to the Egyptian words. If an Egyptian word has a Coptic successor, it is now listed on the word overview page in ORAEC. For example: Go to the above mentioned [preposition r](https://oraec.github.io/corpus/91900.html)! There you can find the link to the Coptic preposition [ⲉ](https://coptic-dictionary.org/entry.cgi?tla=C615).

Until the next blog, which probably won't be very soon as we are working on the next big project!

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a></p>
