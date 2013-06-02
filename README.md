This repo contains human curation data from blekko's slashtag filter
system, which is used to drive the categories in the results on
the blekko.com search engine and izik tablet and phone search apps.

Our hope is that researchers find this data as useful as the Open
Directory Project (dmoz) web directory dataset once was. The founders
of blekko were the founders of NewHoo, the startup which began
the Open Directory Project.

For more details, please see:

http://help.blekko.com/index.php/what-is-a-slashtag/
http://blog.blekko.com/2013/01/14/cracking-the-search-category-problem/

We generate the categories in blekko and izik's search results based
on this human curation data, augmented by machine-learning, and then
applied to the data in the web graph in our web crawl.

We believe that the data in this repo is not copyrightable. As far as
blekko so concerned, you can use it in any way you wish.

You can follow us on Twitter at @blekko or @iziksearch, or send us
email at support@blekko.com

======================================================================

Format of slastags.json

This tag contains the slashtag hierarchy. Each slashtag contains 0 or
more urls and slashtags. The slashtags form a DAG.

URLs come in 3 forms:

1) Complete websites. Example: http://www.gamblersanonymous.org/
2) Paths within a website. Example: http://espn.go.com/nfl/
3) Wildcarded paths. Example: http://www.oscon.com/*perl

