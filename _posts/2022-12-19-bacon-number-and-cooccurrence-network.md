# Bacon number and cooccurrence network

Do you know the Bacon number? No, it's nothing to eat; no, it has nothing to do with Francis Bacon either. It's about the actor [Kevin Bacon](https://en.wikipedia.org/w/index.php?title=Kevin_Bacon&oldid=1127645230). The Bacon number is an illustration of the [small world phenomenon](https://en.wikipedia.org/w/index.php?title=Small-world_experiment&oldid=1126289033), which says that you can contact any person in the world through just six contacts. That's why it's called small world pheonomenon; because whether it's Australia, Bhutan, or Chile, the world moves close together when you only need six contacts.

The Bacon number illustrates this vividly in the world of actors. Every actor who has acted in a film with Kevin Bacon has Bacon number 1. Every actor who has acted with an actor with Bacon number 1, but not with Kevin Bacon, has Bacon number 2. The principle is simple, isn't it?

And the Bacon number illustrates the small world pheonomenon really well, because surprisingly, actors who have nothing to do with Kevin Bacon have a small Bacon number. Bollywood star [Amitabh Bachchan](https://en.wikipedia.org/w/index.php?title=Amitabh_Bachchan&oldid=1127789670) has Bacon number 2 because he played in the movie [The Great Gatsby](https://en.wikipedia.org/w/index.php?title=The_Great_Gatsby_(2013_film)&oldid=1128237075) with [Joel Edgerton](https://en.wikipedia.org/w/index.php?title=Joel_Edgerton&oldid=1127590018). Joel Edgerton, in turn, played in [Black Mass](https://en.wikipedia.org/w/index.php?title=Black_Mass_(film)&oldid=1119341361) with Kevin Bacon. Or the great hero of the silent film era [Douglas Fairbanks](https://en.wikipedia.org/w/index.php?title=Douglas_Fairbanks&oldid=1128134485): he has the Bacon number 3. You can find all this out on the great website <http://www.oracleofbacon.org/>.

So the actors form a huge network. That's the keyword that connects this introduction to ORAEC. In the [blog before last](https://oraec.github.io/2022/12/07/collocations.html), we presented the collocations from the corpus. When two words are used together within a sentence, they form a cooccurrence and thus potentially a collocation. Just as actors are linked when they act together in a movie, lemmas are linked when they are used in a sentence. Based on the cooccurrences, one can form a cooccurrence network. One speaks of nodes or vertices and of egdes. In a cooccurrence network, the nodes are the individual lemmas. Nodes are linked if the lemmas have a cooccurrence. This linkage is called edge.

A common format to represent such a network is the XML based [GraphML](https://en.wikipedia.org/w/index.php?title=GraphML&oldid=1060832076). We have converted the cooccurrences of ORAEC into such a format and published it [here](https://github.com/oraec/corpus_raw_data/blob/main/collocation/cooccurrence.graphml). With suitable software like [Gephi](https://gephi.org/) or [igraph](https://igraph.org/) one can visualize the network and calculate [certain metrics](http://www-math.ucdenver.edu/~wcherowi/courses/m4408/glossary.htm). Get started if you want! The data is CC0! There are even blogs describing the publication of Gephi networks on static pages, cf. e.g. <https://blog.miz.space/tutorial/2020/01/05/gephi-tutorial-sigma-js-plugin-publishing-interactive-graph-online/>. Visualizations are a great thing to show the data vividly. If done well, they show the essentials and hide the uninteresting. We have to confess, we failed at this goal. Our visualizations of the cooccurrence network do not adequately explore the data. This is partly our inability, and partly due to the size of the graph. The network consists of 18733 nodes and 764753 edges. Guys, if you can visualize this nicely, do it! We have to go a different way to describe the network here.

First, let's take some metrics that Gephi calculated for us. The [average path length](https://en.wikipedia.org/w/index.php?title=Average_path_length&oldid=1100899985) is 2.321. The path length describes the shortest path between two nodes. To illustrate the path length: In our cooccurrence network, if two lemmas are directly linked, i.e., used together in a sentence, the path length is 1. If there is a third lemma that is both a cooccurrence partner of one and the other lemma, the path length is 2. Thus, with an average path length of 2.321, one only needs one or two intermediate steps on average to get from one lemma to the next!

The maximum of all shortest paths is called [diameter](https://en.wikipedia.org/w/index.php?title=Network_science&oldid=1126249106). The diameter is 8 in the cooccurence network.

Finally, we adapt the Bacon number for the cooccurrence network. We simply take a lemma to act as the center of the network, as Kevin Bacon does for the network with the Bacon number. We present the Rꜥw number 😉

So the name of the sun god has the Rꜥw number 0. All lemmas used in a sentence with Rꜥw have Rꜥw number 1. These are all the lemmas listed on the <https://oraec.github.io/corpus/collocation_400015.html> page. We have created a [csv](https://github.com/oraec/corpus_raw_data/blob/main/collocation/raw_number.csv) in which the IDs of the lemmas are assigned their Rꜥw number.

The highest assigned Rꜥw number is 5, so it takes at most 5 steps to get to another lemma. Stop! This is not quite true. Have a look at the [csv](https://github.com/oraec/corpus_raw_data/blob/main/collocation/raw_number.csv). There are only 17890 entries with one Rꜥw number listed, but the cooccurrence network consists of 18733 nodes. So 843 lemmas have no Rꜥw number. There is no path to these lemmas from Rꜥw. How is this possible? Let's look at an example: The [personal name Jm.t-wꜣj](https://oraec.github.io/corpus/854073.html) occurs only once in ORAEC: <https://oraec.github.io/corpus/oraec7977-1.html>. This sentence consists only of this very personal name. Thus, the lemma does not have a cooccurrence partner. Accordingly, its node has no edges. There can be no path to Rꜥw at all! Most of these 843 lemmas occur only once, and then in a sentence consisting of only one word. Occasionally, there are sentences consisting of two words, both of which are used exclusively in that sentence, for example: <https://oraec.github.io/corpus/oraec1331-3.html>. Then the network only leads from one lemma to the other and back again! Even then there is no way to Rꜥw.

Another thing you can learn from the Bacon number or the Rꜥw number: It's actually quite easy to lower your Bacon number. All you have to do is shoot a movie with Kevin Bacon, or with an actor with a low Bacon number. Exactly the same is true for the Rꜥw number: one only has to integrate a sentence in ORAEC in which Rꜥw is used together with a lemma that previously had a large Rꜥw number. Then the Rꜥw number is 1 at one time. Whether Rꜥw is used together with a lemma only once in a sentence or more often does not matter for the Rꜥw number. In other cases, however, the frequency of the connection is significant. Statistical significance necessarily operates on frequencies. Therefore, this value is also specified in the [GraphML file](https://github.com/oraec/corpus_raw_data/blob/main/collocation/cooccurrence.graphml).

Finally: <https://oracleofbacon.org/center.php> calculates the average Bacon number. So we can also calculate the average Rꜥw number: (0\*1)+(1\*2646)+(2\*14392)+(3\*793)+(4\*48)+(5\*10) / 17890 = 1.903 Our cooccurrence network presents itself more compact than the actor network around Kevin Bacon. This is not surprising. The diameter of the cooccurrence network is 8, and there are actors with a higher Bacon number than 8! <https://oracleofbacon.org/center.php> also calculates other numbers, which do not take Kevin Bacon, but another actor as starting point, as center. [Samuel L. Jackson](https://en.wikipedia.org/w/index.php?title=Samuel_L._Jackson&oldid=1125952969) has as average value for a Jackson number 2.983. The best center is [Harvey Keitel](https://en.wikipedia.org/w/index.php?title=Harvey_Keitel&oldid=1125581453) with 2.90672, see <https://oracleofbacon.org/center_list.php>. What would then be the best center for the cooccurrence network? This is a nice homework for you in the next few weeks. We are not online during this time, because we are taking a spiritual retreat for the coming Christmas season until mid-January. We wish all our readers a blessed Christmas.

<p xmlns:cc="http://creativecommons.org/ns#" >This work is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a></p>