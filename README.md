# Awesome Dynamic Graphs
A collection of resources on dynamic/streaming/temporal/evolving graph processing systems, databases, data structures, datasets, and related academic and industrial work.

## Contributing
To add, remove or change things on the list:
[please submit a pull request to the GitHub repository](https://github.com/domargan/awesome-dynamic-graphs).


## Open Source Projects
### Data Structures, Systems and Frameworks
* [Aspen](https://github.com/ldhulipala/aspen) [C++]
    * Streaming graph processing system based on compressed purely-functional trees
    * [Paper](https://people.csail.mit.edu/jshun/aspen.pdf)
* [Differential Dataflow](https://github.com/frankmcsherry/differential-dataflow) [Rust]
    * General data-parallel programming framework suitable for processing large dynamic graphs
    * [Paper](http://michaelisard.com/pubs/differentialdataflow.pdf)
* [GraphBolt](https://github.com/pdclab/graphbolt) [C++]
    * Streaming graph processing system that provides BSP guarantees 
    * [Paper](https://dl.acm.org/doi/10.1145/3302424.3303974)
* [GraphJet](https://github.com/twitter/GraphJet) [Java]
    * Streaming graph processing system for generating content recommendations at Twitter
    * [Paper](https://www.vldb.org/pvldb/vol9/p1281-sharma.pdf)
* [GraphOne](https://github.com/the-data-lab/GraphOne) [C++]
    * Storage engine for streaming graph data
    * [Paper](https://www.usenix.org/system/files/fast19-kumar.pdf)
* [GreyCat](https://github.com/datathings/greycat) [Java]
    * _Many-world_ temporal graph data store
    * [Paper](https://hal.inria.fr/hal-02059882/document)
* [GoFFish](https://github.com/usc-cloud/goffish)[Java]
    * Multi-source streaming graph processing system
* [KickStarter](https://github.com/pdclab/graphbolt)[C++]
    * Streaming graph processing system optimising for path-based/monotonic graph algorithms
    * [Paper](https://dl.acm.org/doi/10.1145/3037697.3037748)
* [LLAMA](https://github.com/goatdb/llama) [C++]
    * CSR-based storage engine and streaming graph processing system
    * [Paper](https://ieeexplore.ieee.org/document/7113298/)
* [PCSR](https://github.com/wheatman/Packed-Compressed-Sparse-Row/) [C++]
    * CSR-inspired, packed memory array based data structure for streaming graphs
    * [Paper](https://ieeexplore.ieee.org/document/8547566)
* [PPCSR](https://github.com/domargan/parallel-packed-csr) [C++]
    * Parallel and NUMA-aware implementation of PCSR data structure for streaming graphs
* [Raphtory](https://github.com/Raphtory/Raphtory) [Scala]
    * Snapshot-based distributed streaming graph processing system
    * [Paper](https://www.sciencedirect.com/science/article/pii/S0167739X19301621)
* [STINGER](https://github.com/stingergraph/stinger) [C/C++]
    * Data structure for streaming graphs based on linked lists of blocks
    * [Paper](https://ieeexplore.ieee.org/document/6408680)
* [Temporal Ligra](https://github.com/jshun/ligra/tree/temporal) [C++]
    * Minimal version of Ligra graph processing system for static temporal graphs.
    * Temporal CSR data structure: supports graphs where edges have both weights and time intervals.
    * Includes example parallel implementation of [temporal SSSPs and betweeness centralities](https://github.com/jshun/ligra/blob/temporal/apps/temporal/).

### Benchmarking
* [GraphTides](https://github.com/GraphTides/graphtides) [Java/TypeScript]
    * Framework for evaluating streaming graph processing platforms
    * [Paper](https://dl.acm.org/doi/10.1145/3210259.3210262)


## Papers
Check [Julian Shun's list](https://people.csail.mit.edu/jshun/graph.shtml#streamingframeworks) for a further reference and an extensive collection of related papers.

### Data Structures and Storage
[STINGER: Spatio-Temporal Interaction Networks and Graphs (STING) Extensible Representation](https://pdfs.semanticscholar.org/6992/7a3b9fc25e655ce662c03deb1e9d2832585c.pdf)  (2009)

[STINGER: High Performance Data Structure for Streaming Graphs](https://ieeexplore.ieee.org/document/6408680)  (HPEC 2012)

[Packed Compressed Sparse Row: A Dynamic Graph Representation](https://ieeexplore.ieee.org/document/8547566) (HPEC 2018)

[GraphOne: A Data Store for Real-time Analytics on Evolving Graphs](https://dl.acm.org/doi/abs/10.1145/3364180) (FAST 2019)

[GraphTinker: A High Performance Data Structure for Dynamic Graph Processing](https://ieeexplore.ieee.org/abstract/document/8821003) (IPDPS 2019)

[CSR++: A Fast, Scalable, Update-Friendly Graph DataStructure](https://hal.archives-ouvertes.fr/hal-03060095/document) (OPODIS 2020)

[LiveGraph: A Transactional Graph Storage System With Purely Sequential Adjacency List Scans](https://dl.acm.org/doi/abs/10.14778/3384345.3384351) (VLDB 2020)

[A Parallel Packed Memory Array to Store Dynamic Graphs](https://epubs.siam.org/doi/pdf/10.1137/1.9781611976472.3) (ALENEX 2021)

### Systems and Frameworks
[STINGER: Spatio-Temporal Interaction Networks and Graphs (STING) Extensible Representation](https://pdfs.semanticscholar.org/6992/7a3b9fc25e655ce662c03deb1e9d2832585c.pdf)  (2009)

[On Querying Historical Evolving Graph Sequences](http://www.vldb.org/pvldb/vol4/p726-ren.pdf)  (VLDB 2011)

[STINGER: High Performance Data Structure for Streaming Graphs](https://ieeexplore.ieee.org/document/6408680)  (HPEC 2012)

[Facilitating Real-Time Graph Mining](https://dl.acm.org/citation.cfm?id=2390023)  (CloudDB 2012)

[Kineograph: Taking the Pulse of a Fast-Changing and Connected World](https://dl.acm.org/citation.cfm?id=2168846)  (EuroSys 2012)

[Differential Dataflow](http://cidrdb.org/cidr2013/Papers/CIDR13_Paper111.pdf)  (CIDR 2013)

[Efficient Snapshot Retrieval over Historical Graph Data](https://ieeexplore.ieee.org/document/6544892)  (ICDE 2013)

[Naiad: A Timely Dataflow System](https://dl.acm.org/citation.cfm?id=2522738)  (SOSP 2013)

[Chronos: A Graph Engine for Temporal Graph Analysis](https://dl.acm.org/citation.cfm?id=2592799)  (EuroSys 2014)

[Towards Large-Scale Graph Stream Processing Platform](https://dl.acm.org/citation.cfm?id=2580051)  (WWW 2014)

[CellIQ : Real-Time Cellular Network Analytics at Scale](https://www.usenix.org/system/files/conference/nsdi15/nsdi15-paper-iyer.pdf)  (NSDI 2015)

[DISTINGER: A Distributed Graph Data Structure for Massive Dynamic Graph Processing](https://ieeexplore.ieee.org/document/7363954)  (Big Data 2015)

[ImmortalGraph: A System for Storage and Analysis of Temporal Graphs](https://dl.acm.org/citation.cfm?id=2700302)  (Transactions on Storage 2015)

[LLAMA: Efficient Graph Analytics Using Large Multiversioned Arrays](https://ieeexplore.ieee.org/document/7113298/)  (ICDE 2015)

[Real-time Analytics for Fast Evolving Social Graphs](https://ieeexplore.ieee.org/document/7152566)  (CCGrid 2015)

[GraphIn: An Online High Performance Incremental Graph Processing Framework](https://link.springer.com/chapter/10.1007%2F978-3-319-43659-3_24)  (Euro-Par 2016)

[GraphJet: Real-Time Content Recommendations at Twitter](https://dl.acm.org/citation.cfm?id=3007267)  (VLDB 2016)

[Storing and Analyzing Historical Graph Data at Scale](http://openproceedings.org/2016/conf/edbt/paper-29.pdf)  (EDBT 2016)

[Synergistic Analysis of Evolving Graphs](https://dl.acm.org/citation.cfm?id=2992784)  (TACO 2016)

[Time-Evolving Graph Processing at Scale](https://dl.acm.org/citation.cfm?id=2960419)  (GRADES 2016)

[Tornado: A System For Real-Time Iterative Analysis Over Evolving Data](https://dl.acm.org/citation.cfm?id=2882903.2882950)  (SIGMOD 2016)

[Towards a Distributed Large-Scale Dynamic Graph Data Store](https://ieeexplore.ieee.org/document/7529955)  (IPDPSW 2016)

[Automatic Algorithm Transformation for Efficient Multi-Snapshot Analytics on Temporal Graphs](https://dl.acm.org/citation.cfm?id=3090166)  (VLDB 2017)

[KickStarter: Fast and Accurate Computations on Streaming Graphs via Trimmed Approximations](https://dl.acm.org/doi/10.1145/3037697.3037748) (ASPLOS 2017) 

[Auxo: A Temporal Graph Management System](https://ieeexplore.ieee.org/document/8486795) (BDMA 2018)

[Distributed Evaluation of Subgraph Queries Using Worst-case Optimal Low-Memory Dataflows](https://dl.acm.org/citation.cfm?id=3199520)  (VLDB 2018)

[GraPU: Accelerate Streaming Graph Analysis through Preprocessing Buffered Updates](https://dl.acm.org/citation.cfm?id=3267811)  (SOCC 2018)

[GraphBolt: Dependency-Driven Synchronous Processing of Streaming Graphs](https://dl.acm.org/citation.cfm?id=3303974)  (EuroSys 2019)

[Low-Latency Graph Streaming Using Compressed Purely-Functional Trees](https://people.csail.mit.edu/jshun/aspen.pdf) (PLDI 2019)

[GraphOne: A Data Store for Real-time Analytics on Evolving Graphs](https://dl.acm.org/doi/abs/10.1145/3364180) (FAST 2019)

[LiveGraph: A Transactional Graph Storage System With Purely Sequential Adjacency List Scans](https://dl.acm.org/doi/abs/10.14778/3384345.3384351) (VLDB 2020)

[Raphtory: Streaming analysis of distributed temporal graphs](https://www.sciencedirect.com/science/article/pii/S0167739X19301621) (FGCS 2020)

[RisGraph: A Real-Time Streaming System for Evolving Graphs](https://arxiv.org/abs/2004.00803) (2020)

[Tegra: Efficient Ad-Hoc Analytics on Time-Evolving Graphs]() (NSDI 2021)

### Surveys
[The Ubiquity of Large Graphs and Surprising Challenges of Graph Processing](https://dl.acm.org/doi/abs/10.1145/3164135.3164139) (VLDB 2018)

[Practice of Streaming and Dynamic Graphs: Concepts, Models, Systems, and Parallelism](https://www.research-collection.ethz.ch/handle/20.500.11850/462546) (2020)

## Datasets
Note: Very small datasets are not included in the list.
|        Category        	|        Data Source        	|           Name          	|          Type          	|   Vertex Meaning  	|      Edge Meaning     	| Size (\|V\|) 	| Volume (\|E\|) 	| Edge Weight 	| Edge Timestamps 	| Multiple Edges 	|                     Source/Link                    	|
|:----------------------:	|:-------------------------:	|:-----------------------:	|:----------------------:	|:-----------------:	|:---------------------:	|:------------:	|:--------------:	|:-----------:	|:---------------:	|:--------------:	|:--------------------------------------------------:	|
|   Authorship network   	|         Wikipedia         	|       edit-enwiki       	|  Bipartite, undirected 	|   User, article   	|          Edit         	|  50,757,442  	|   572,591,272  	|      N      	|        Y        	|        Y       	|       http://konect.cc/networks/edit-enwiki/       	|
|    Citation network    	|            DBLP           	|        dblp-cite        	|  Unipartite, directed  	|    Publication    	|        Citation       	|    12,590    	|     49,759     	|      N      	|        Y        	|        N       	|        http://konect.cc/networks/dblp-cite/        	|
|   Co-citation network  	|           arXiv           	|       ca-cit-HepPh      	| Unipartite, undirected 	|       Author      	|      Co-citation      	|    28,093    	|    4,596,803   	|      N      	|        Y        	|        Y       	|       http://konect.cc/networks/ca-cit-HepPh/      	|
|   Co-citation network  	|           arXiv           	|       ca-cit-HepTh      	| Unipartite, undirected 	|       Author      	|      Co-citation      	|    22,908    	|    2,673,133   	|      N      	|        Y        	|        Y       	|       http://konect.cc/networks/ca-cit-HepTh/      	|
|  Communication network 	|          Facebook         	|    facebook-wosn-wall   	|  Unipartite, directed  	|        User       	|       Wall post       	|    46,952    	|     876,993    	|      N      	|        Y        	|        Y       	|    http://konect.cc/networks/facebook-wosn-wall/   	|
|  Communication network 	| Linux kernel mailing list 	|        lkml-reply       	|  Unipartite, directed  	|       Person      	|         Reply         	|    63,399    	|    1,096,440   	|      N      	|        Y        	|        Y       	|        http://konect.cc/networks/lkml-reply/       	|
|    Computer network    	|     Internet topology     	|         topology        	| Unipartite, undirected 	| Autonomous system 	|       Connection      	|    34,761    	|     171,403    	|      N      	|        Y        	|        Y       	|         http://konect.cc/networks/topology/        	|
|     Feature network    	|         BibSonomy         	|      bibsonomy-2ti      	|  Bipartite, undirected 	|  Tag, publication 	|       Assignment      	|    972,120   	|    2,555,080   	|      N      	|        Y        	|        Y       	|      http://konect.cc/networks/bibsonomy-2ti/      	|
|     Feature network    	|         CiteULike         	|       citeulike-ti      	|  Bipartite, undirected 	|  Tag, publication 	|       Assignment      	|    885,046   	|    2,411,819   	|      N      	|        Y        	|        Y       	|       http://konect.cc/networks/citeulike-ti/      	|
|     Feature network    	|         Delicious         	|       delicious-ti      	|  Bipartite, undirected 	|     Tag,  URL     	|     Tag assignment    	|  38,289,740  	|   301,183,605  	|      N      	|        Y        	|        Y       	|       http://konect.cc/networks/delicious-ti/      	|
|     Feature network    	|          Google+          	|    stevgong_attribute   	|  Bipartite, undirected 	|  User, attribute  	|     Attribute-link    	|  10,442,421  	|   20,592,962   	|      N      	|        Y        	|        N       	|    http://konect.cc/networks/stevgong_attribute/   	|
|     Feature network    	|          Twitter          	|   munmun_twitterex_ti   	|  Bipartite, undirected 	|   Hashtag,  URL   	|     Co-occurrence     	|   1,502,611  	|    2,635,885   	|      N      	|        Y        	|        Y       	|   http://konect.cc/networks/munmun_twitterex_ti/   	|
|  Human contact network 	|            MIT            	|           mit           	| Unipartite, undirected 	|       Person      	|        Contact        	|      96      	|    1,086,404   	|      N      	|        Y        	|        Y       	|           http://konect.cc/networks/mit/           	|
|    Hyperlink network   	|         Wikipedia         	|   link-dynamic-dewiki   	|  Unipartite, directed  	|      Article      	|       Reference       	|   2,166,669  	|   86,337,879   	|      N      	|        Y        	|        N       	|   http://konect.cc/networks/link-dynamic-dewiki/   	|
|    Hyperlink network   	|         Wikipedia         	|   link-dynamic-frwiki   	|  Unipartite, directed  	|      Article      	|       Reference       	|   2,212,682  	|   59,008,831   	|      N      	|        Y        	|        N       	|   http://konect.cc/networks/link-dynamic-frwiki/   	|
|    Hyperlink network   	|         Wikipedia         	|   link-dynamic-itwiki   	|  Unipartite, directed  	|      Article      	|       Reference       	|   1,204,009  	|   34,826,283   	|      N      	|        Y        	|        N       	|   http://konect.cc/networks/link-dynamic-itwiki/   	|
|    Hyperlink network   	|         Wikipedia         	|   link-dynamic-nlwiki   	|  Unipartite, directed  	|      Article      	|       Reference       	|   1,039,252  	|   20,070,561   	|      N      	|        Y        	|        N       	|   http://konect.cc/networks/link-dynamic-nlwiki/   	|
|    Hyperlink network   	|         Wikipedia         	|   link-dynamic-plwiki   	|  Unipartite, directed  	|      Article      	|       Reference       	|   1,033,050  	|   25,026,208   	|      N      	|        Y        	|        N       	|   http://konect.cc/networks/link-dynamic-plwiki/   	|
|    Hyperlink network   	|         Wikipedia         	| link-dynamic-simplewiki 	|  Unipartite, directed  	|      Article      	|       Reference       	|    100,312   	|    1,627,472   	|      N      	|        Y        	|        N       	| http://konect.cc/networks/link-dynamic-simplewiki/ 	|
|   Interaction network  	|           LastFm          	|       lastfm_band       	|  Bipartite, undirected 	|     User, band    	|       Listening       	|    175,069   	|   19,150,868   	|      N      	|        Y        	|        Y       	|       http://konect.cc/networks/lastfm_band/       	|
|   Interaction network  	|           LastFm          	|       lastfm_song       	|  Bipartite, undirected 	|     User, song    	|       Listening       	|   1,085,612  	|   19,150,868   	|      N      	|        Y        	|        Y       	|       http://konect.cc/networks/lastfm_song/       	|
| Online contact network 	|       Stack Exchange      	|       sx-askubuntu      	|  Unipartite, directed  	|        User       	|     Answer/comment    	|    159,316   	|     964,437    	|      N      	|        Y        	|        Y       	|       http://konect.cc/networks/sx-askubuntu/      	|
| Online contact network 	|       Stack Exchange      	|     sx-mathoverflow     	|  Unipartite, directed  	|        User       	|     Answer/comment    	|    24,818    	|     506,550    	|      N      	|        Y        	|        Y       	|     http://konect.cc/networks/sx-mathoverflow/     	|
| Online contact network 	|       Stack Exchange      	|     sx-stackoverflow    	|  Unipartite, directed  	|        User       	|     Answer/comment    	|   2,601,977  	|   63,497,050   	|      N      	|        Y        	|        Y       	|     http://konect.cc/networks/sx-stackoverflow/    	|
| Online contact network 	|       Stack Exchange      	|       sx-superuser      	|  Unipartite, directed  	|        User       	|     Answer/comment    	|    194,085   	|    1,443,339   	|      N      	|        Y        	|        Y       	|       http://konect.cc/networks/sx-superuser/      	|
| Online contact network 	|          Twitter          	|      higgs-twitter      	|  Unipartite, directed  	|        User       	| Retweet/mention/reply 	|       ?      	|     563,069    	|      N      	|        Y        	|      Y (?)     	|  https://snap.stanford.edu/data/higgs-twitter.html 	|
| Online contact network 	|          Twitter          	|   munmun_twitterex_at   	|  Unipartite, directed  	|        User       	|        Mention        	|   2,919,613  	|   12,887,063   	|      N      	|        Y        	|        Y       	|   http://konect.cc/networks/munmun_twitterex_at/   	|
| Online contact network 	|         Wikipedia         	|           elec          	|  Unipartite, directed  	|        User       	|          Vote         	|     7,118    	|     103,675    	|      N      	|        Y        	|        N       	|           http://konect.cc/networks/elec/          	|
| Online contact network 	|         Wikipedia         	|       wikiconflict      	| Unipartite, undirected 	|        User       	|     Edit conflict     	|    118,100   	|    2,917,785   	|      Y      	|        Y        	|        Y       	|       http://konect.cc/networks/wikiconflict/      	|
|  Online social network 	|          Bitcoin          	|       soc-bitcoin       	|  Unipartite, directed  	|       Member      	|     Trust/distrust    	|  24,575,382  	|   122,948,162  	|      ?      	|        Y        	|        N       	|    https://networkrepository.com/soc-bitcoin.php   	|
|  Online social network 	|            Digg           	|       digg-friends      	|  Unipartite, directed  	|        User       	|          Vote         	|    279,630   	|    1,731,653   	|      N      	|        Y        	|        N       	|       http://konect.cc/networks/digg-friends/      	|
|  Online social network 	|          Facebook         	|   facebook-wosn-links   	| Unipartite, undirected 	|        User       	|       Friendship      	|    63,731    	|     817,035    	|      N      	|        Y        	|        N       	|   http://konect.cc/networks/facebook-wosn-links/   	|
|  Online social network 	|           Flickr          	|      flickr-growth      	|  Unipartite, directed  	|        User       	|       Friendship      	|   2,302,925  	|   33,140,017   	|      N      	|        Y        	|        N       	|      http://konect.cc/networks/flickr-growth/      	|
|  Online social network 	|          Google+          	|     stevgong_social     	|  Unipartite, directed  	|        User       	|      Interaction      	|  28,943,739  	|   462,994,069  	|      N      	|        Y        	|        N       	|     http://konect.cc/networks/stevgong_social/     	|
|  Online social network 	|          YouTube          	|     youtube-u-growth    	| Unipartite, undirected 	|        User       	|       Friendship      	|   3,223,589  	|    9,375,374   	|      N      	|        Y        	|        N       	|     http://konect.cc/networks/youtube-u-growth/    	|
|     Rating network     	|           Amazon          	|      rec-amz-Books      	|  Bipartite, undirected 	|   User, product   	|         Rating        	|  10,356,390  	|   22,507,155   	|      Y      	|        Y        	|        N       	|   https://networkrepository.com/rec-amz-Books.php  	|
|     Rating network     	|          Epinions         	|     epinions-rating     	|  Bipartite, undirected 	|   User, product   	|         Rating        	|    876,252   	|   13,668,320   	|      N      	|        Y        	|        Y       	|     http://konect.cc/networks/epinions-rating/     	|
|     Rating network     	|          Netflix          	|         netflix         	|  Bipartite, undirected 	|    User, movie    	|         Rating        	|    497,959   	|   100,480,507  	|      Y      	|        Y        	|        N       	|         http://konect.cc/networks/netflix/         	|
|     Rating network     	|           Yahoo           	|        yahoo-song       	|  Bipartite, undirected 	|    Person, song   	|         Rating        	|   1,625,951  	|   256,804,235  	|      Y      	|        Y        	|        N       	|        http://konect.cc/networks/yahoo-song/       	|



## About
This list was compiled by [Domagoj Margan](https://github.com/domargan) with help and resources from the systems community.
