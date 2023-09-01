# CC-BY requires stable bibliographic data

## Intro

Hi folks! We are starting our blog with an appeal for donations. There is a site on the net that is really central and depends on your donations. It's <https://archive.org/> It's really the central archive of the Internet, where you can find old versions of web pages, among other things:

![Wayback Machine](/img/blog/waybackmachine.jpg "Wayback Machine")

As this blog progresses, it will become clear why we are mentioning this site today. Okay, let's get started.

Licenses are the backbone of data reuse because they provide legal certainty: what is allowed with what data, and what is not? And rights holders can define exactly how their data can be reused. We already had a [separate blog entry on Creative Commons](https://oraec.github.io/2022/11/30/cc-by-sa-an-cc0.html). Given the occasion, we need to shed some light on the BY here. This abbreviation means that you have to give credit to the authors of the data when it is reused. Here is an example: Anne creates some data. So she owns the copyright of this data. She makes this data available under the CC-BY license. This means that anyone can reuse her data under exactly one condition: It must be acknowledged that Anne is the author of the data. Think of it this way: Anne puts her data in a package and puts a label on it. The label contains the license and author information. Anne then releases the package to the public so that people can reuse it. Then the Reuse Company comes along and thinks Anne's data is excellent. The Reuse Company packages its own package that includes Anne's data and other data. The Reuse Company also releases the new package into the public domain, and puts Anne's license and author information on it as a label. Got it? It works the same way with reused data on the Internet. Someone makes something available, and someone else publishes something new. For this to work smoothly, two things are needed: trust and stability. What does that mean, and what problems might arise?

### Stability of the data

Let's stay with the example! Imagine the following: After the Reuse Company has created its package with Anne's data (license-compliant!), Anne goes to your package and changes her data that is in it. So we have two versions of the data: the original one that is in the Reuse Company's package, and the modified one that is in Anne's package. Anne has licensed her data under the CC-BY license. Therefore, the Reuse Company also credits Anne as the author. But now Anne can claim that the Reuse Company is distributing data under Anne's name that does not come from Anne at all. She is referring to her package, which, according to the Reuse Company, is the basis for the Reuse Company's package, but which, after Anne's modification, contains completely different data. Do you see the problem? Legally compliant reuse is only possible if the data provided remains stable. Subsequent changes must not be allowed. Today, this is standard for all vendors. Behind a DOI is always the same thing. This guarantee by the provider that the data will remain stable creates the trust that makes reuse possible in the first place. So our constructed example is not even possible. Anne cannot change the contents of her package at all. It's locked and no one can change it. Thank goodness!

### Metadata Stability

Okay, Anne can no longer change her data. She can no longer open her package. But there is another problem. Imagine that Anne looks at the label of her package and realizes that she misspelled her name. What do you think? Can she change the label? Anne would have your sympathy in this case, wouldn't she? Only if the name is spelled correctly does the author information make sense, right? But she might want to change more than that: She could write on the sticker that she did not create the data alone, but that she created it together with Paul. This would have serious implications for the BY. So if Anne changes the author statement, the Reuse Company would no longer have the notation that is on the original package. Now Anne and Paul can claim that the Reuse Company is violating the license terms. You see, even with metadata, you need stability, otherwise reuse is dangerous. And the ability to change the metadata is real! We will show you an example:

## Changing the bibliographic data

As explained in our blog, we reuse a particular dataset to represent the hierarchy of our corpus data. We cite it as follows: [Teilauszug der Datenbank des Vorhabens "Strukturen und Transformationen des Wortschatzes der ägyptischen Sprache" vom Januar 2018](https://nbn-resolving.org/urn:nbn:de:kobv:b4-opus4-29190) The following is currently hidden behind the link:

![teilauszug today](/img/blog/teilauszug_2023.jpg "teilauszug today")

and

![teilauszug metadata today](/img/blog/teilauszug_metadata_2023.jpg "teilauszug metadata today")

If you download the data as Bibtex, you get:

```
@misc{OPUS4-2919,
  title     = {Teilauszug der Datenbank des Vorhabens "Strukturen und Transformationen des Wortschatzes der {\"a}gyptischen Sprache" vom Januar 2018},
  editor    = {Tonio Sebastian Richter and Ingelore Hafemann and Hans-Werner Fischer-Elfert and Peter Dils},
  institution = {Akademienvorhaben Strukturen und Transformationen des Wortschatzes der {\"a}gyptischen Sprache. Text- und Wissenskultur im alten {\"A}gypten},
  type      = {researchdata},
  year        = {2018},
}
```

So there are editors we don't name and a recommended citation we don't follow. When we saw this, we wondered a lot. Fortunately, there is the <https://archive.org/> mentioned above. If you type the URL <https://edoc.bbaw.de/frontdoor/index/index/docId/2919> into the Wayback Machine, you can see previous versions of the site. The [oldest](https://web.archive.org/web/20200716075024/https://edoc.bbaw.de/frontdoor/index/index/docId/2919) is from 2020:

![teilauszug original](/img/blog/teilauszug_2020.jpg "teilauszug original")

and

![teilauszug metadata original](/img/blog/teilauszug_metadata_2020.jpg "teilauszug metadata original")

You can even download the old data in bibtex format, see <https://web.archive.org/web/20210804141042/https://edoc.bbaw.de/citationExport/index/download/docId/2919/output/bibtex>. They look like this:

```
@misc{OPUS4-2919,
  title     = {Teilauszug der Datenbank des Vorhabens "Strukturen und Transformationen des Wortschatzes der {\"a}gyptischen Sprache" vom Januar 2018},
  institution = {Akademienvorhaben Strukturen und Transformationen des Wortschatzes der {\"a}gyptischen Sprache. Text- und Wissenskultur im alten {\"A}gypten},
  type      = {other},
  year        = {2018},
}
```

With the help of the Wayback Machine service, one can clearly prove that the bibliographic data have changed. Initially, there was no citation note, there were no editors, and finally, the institution responsible for the data was different: the Saxon Academy (SAW) was added later. The change took place between October 1, 2022 and March 4, 2023, as the two Wayback Machine snapshots suggest: <https://web.archive.org/web/20221001024837/https://edoc.bbaw.de/frontdoor/index/index/docId/2919> and <https://web.archive.org/web/20230304173725/https://edoc.bbaw.de/frontdoor/index/index/docId/2919>. This fits well with our recollection that no editors were named in our download.

## Evaluation of the change

Now, the reason for the change can be two things: First, it may be an error correction. Something was forgotten, which was subsequently corrected. Second, it may be a subsequent adjustment to the current policy. The old TLA was issued by Berlin Academy (BBAW) alone, see <https://aaew.bbaw.de/tla/impressum.html>. But the [new TLA](https://thesaurus-linguae-aegyptiae.de/legal/imprint?lang=en) lists scientific editors belonging to both BBAW and SAW. This joint responsibility is also reflected in the subsequently changed bibliographic data. In the following, we will show that the evidence strongly supports the second variant, i.e. that this is not an error correction, but a deliberate change and deviation from the original metadata.

The academies account for their work by publishing work reports, called "Jahrbuch". The BBAW "Jahrbuch" for 2018 is available online: <https://nbn-resolving.org/urn:nbn:de:kobv:b4-opus4-32676> Here, each project reports on what it has researched and published this year. On page 121 the publications of the project "Strukturen und Transformationen des Wortschatzes der ägyptischen Sprache. Text- und Wissenskultur im Alten Ägypten". The publication of the research data is mentioned as follows:

> Teilauszug der Datenbank des Vorhabens vom Januar 2018, urn:nbn:de:kobv:b4-opus4-29190 (https://edoc.bbaw.de/frontdoor/index/index/docId/2919).

No editor is named here. In other publications, however, an editor is named. In this respect, the absence of a citation is not due to a specific citation policy. In addition, the report states on page 120:

> Überdies wurden Konkordanzen für die Einpflege unserer Daten in externe Datenbestände (THOT – Thesauri&Ontology/Liège) erstellt sowie Rohdaten unserer Datenbank für fachfremde Nutzer (Hieroglyphics Initiative/London) verfügbar gemacht.

The second part of this sentence explicitly refers to the publication of the research data. We note: The "Jahrbuch" agrees with the original version of the bibliographic data that there is no explicit editor. There is no mention of collaboration with SAW in the publication.

The SAW "Jahrbuch" is not available online. We looked at the printed book (ISBN:978-3-7776-2784-7). There was a CD-ROM included! Wow, do you still have a reader to get such data? Anyway, on the CD is a PDF with the detailed seven-page report of this project at SAW. Not a word about the publication of the research data.

In the subsequent SAW "Jahrbuch" (978-3-9823337-0-0) there is also no reference to the research data publication. The section on digital publishing is also interesting. On pages 240-241 it says:

> Soweit es die Sächsische Akademie betrifft, gibt es allerdings kaum den vollständigen Verzicht auf eine gedruckte Veröffentlichung; bislang beschreitet einzig das Projekt "Strukturen und Transformationen des Wortschatzes der ägyptischen Sprache" mit seiner Internetveröffentlichung *Science in Ancient Egypt* diesen Weg.

Here, too, there is no reference to the publication of research data and, incidentally, no reference to the publication platform TLA.

There is also no reference to the research data publication in the [list of publications](https://doi.org/10.1515/9783110629705-002) by Hans-Werner Fischer-Elfert. Since it is from 2019 and contains not only printed articles but also other things (cf. numbers 150 ff.), it does not seem very likely that Hans-Werner Fischer-Elfert is the editor of the research data published in 2018.

All the external data listed indicate that the research data originally had no editor. Similarly, all the evidence suggests that SAW was not involved in the production of the dataset, but that it is solely a production of BBAW. Of course, there are things in the data that were produced at SAW. But if authorship is to be the criterion for the field "creating corporation", then the other institutions, such as the Book of the Dead Project, should also be mentioned.

### Conclusion

So the correct metadata for <https://nbn-resolving.org/urn:nbn:de:kobv:b4-opus4-29190> are the original metadata. They are:

```
@misc{OPUS4-2919,
  title     = {Teilauszug der Datenbank des Vorhabens "Strukturen und Transformationen des Wortschatzes der {\"a}gyptischen Sprache" vom Januar 2018},
  institution = {Akademienvorhaben Strukturen und Transformationen des Wortschatzes der {\"a}gyptischen Sprache. Text- und Wissenskultur im alten {\"A}gypten},
  type      = {other},
  year        = {2018},
}
```

The editor's reference is an after-the-fact invention. It should not be used when citing this research data.

## Summary

Digital licenses require stability not only of the data, but also of the metadata. If bibliographic data changes, this leads to problems in reuse. Our request to libraries: be transparent when you change bibliographic data, and please leave the original versions of the bibliographic data online!

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a></p>
