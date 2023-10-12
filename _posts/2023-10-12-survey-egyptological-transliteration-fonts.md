# Survey: Egyptological Transliteration Fonts

What is the constant in our posts? Maybe we should say "Unicode"! Our first substantial [blog](https://oraec.github.io/2022/09/28/recommendations-encoding-hieroglyphs.html) was about Unicode.  And today, Unicode is still the central point!

What is it all about? Recently, there was a mail on the [EEF list](https://www.egyptologyforum.org/EEFNEWS.html) announcing the update of a font called [Trlit_CG Times](https://oeb.griffith.ox.ac.uk/fonts.aspx). It said:

> The new version, also developed by Willem Hovestreydt, now includes a new character. This is "ï" (i + diaeresis / Unicode: U+00EF), which represents the two oblique strokes usually rendered as "y" (Gardiner Z4) and is inserted by pressing capital Y. 

Can you guess? This is indeed not a Unicode font! If you type a "Y", it will store a "Y", but the font will display it on the interface as if it were an ï. You can easily tell if the font is a Unicode font or if it is just tricking you. Create a transliterated text with the font in question. Then change the font to, let's say, Arial. If the transliteration characters become normal letters like Y or A, then it is not a Unicode font. Then the font is just pretending to have a transliteration.

This was common practice before Unicode. In the age of Unicode, of course, this practice is not quite as understandable. It has serious drawbacks: The data is font-dependent. If you use a different font, you get something different. If you google for ï, the data you entered with a Y will of course not be found.

Okay, we wanted to dismiss this mail as a curiosity. But then we noticed that Egyptology still relies on such non-Unicode fonts. Here are some examples:

The guidelines for the Proceedings of the International Congress of Egyptologists write:

> Use the standard transliteration font Trlit_CG Times for transliterations/transcriptions, and the Coptic_Normal font for Coptic text – the latter two can be downloaded from the Online Egyptological Bibliography website: https://oeb.griffith.ox.ac.uk/fonts.aspx. (<https://ice2023.com/cache/guidelines-english-4-october-2023.2079/guidelines-english-4-october-2023.pdf>)

Guidelines of the Journal:

> All transliterations must be rendered in the Trlit_CG Times font (free to download online) within the text. (<https://journals.sagepub.com/author-instructions/EGA>) 

Guidelines of the Zeitschrift:

> If you make use of other transcription fonts than “Transliteration” or “Umschrift”, please submit them in conjunction with the manuscript. (<https://www.gkr.uni-leipzig.de/fileadmin/Fakult%C3%A4t_GKR/%C3%84gyptologisches_Institut/Dokumente/Guidelines.pdf>)

At least IFAO uses Unicode, see <https://www.ifao.egnet.net/publications/publier/outils-ed/polices/>. Digital projects (from AED to Wikisource, see our compilation <https://oraec.github.io/2023/08/24/leiden-unified-transliteration.html>) also use Unicode.

Confusing, isn't it? That's why we want to get an overview and have created a survey. We would like to know from you who uses which font. We also want to know what continent you are from and how old you are. There is a prejudice in our group that boomers don't use Unicode. We would like to disprove that. Okay, let's go! Here is the [survey](https://tripetto.app/run/UO4SQ6UOME). We will get back to you with the results!

Link of the survey: <https://tripetto.app/run/UO4SQ6UOME>

Perhaps, we can embed the survey. If you only see HTML tags, click the link!

<div id="tripetto-1gqja2"></div>
<script src="https://cdn.jsdelivr.net/npm/@tripetto/runner"></script>
<script src="https://cdn.jsdelivr.net/npm/@tripetto/runner-classic"></script>
<script src="https://cdn.jsdelivr.net/npm/@tripetto/studio"></script>
<script>
TripettoStudio.form({
    runner: TripettoClassic,
    token: "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyIjoiOUhMYzBMb0tOSG9DSTJTUjdJeGxUaTk0OEd4ZElPa1lseXFSUGYxalFYND0iLCJkZWZpbml0aW9uIjoiajhieDVNMkVyRWVsZTc2TDhma1Z5RnNFL0U1ZzBDSkNSNk5QL3ZvUXgwRT0iLCJ0eXBlIjoiY29sbGVjdCJ9.xf57mVWg0m5mljxITqgFYEr1WoMFlV8LkXQXqQBVRqA",
    element: "tripetto-1gqja2"
});
</script>

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a></p>
