# Graph_related


# Graph-Analysis-Papers-Reading-Roadmap


## 1.0 Similarity

**[1]** Fang Y, Lin W, Zheng V W, et al. "**Semantic proximity search on graphs with metagraph-based learning[C]**."  IEEE International Conference on Data Engineering. IEEE, 2016:277-288. [[pdf]](https://www.researchgate.net/publication/303549558_Semantic_Proximity_Search_on_Graphs_with_Metagraph-based_Learning) :star::star::star:

>在图的顶点被分为不同的类别时（即，图上的顶点是“异构”的），这篇文章提出一个计算一个给定顶点在给定的某种语义下与其最“联系紧密”的节点的方法。在现实生活中，如果将人们的社交活动构建为一个图的话，其顶点是由不同种类的顶点构成的，即图的顶点往往是属于不同类别的。由于图中每个顶点都有其特定类别，因此可以通过构造一种固定的结构来表示节点间的关系。我们叫这种结构“metagraphs”，从而把具体对象抽象为其所属类别。利用mentagraph，可以找出在特定的语义下与给定节点最为紧密的节点（例如：与Alice最亲密的“同学”，以及最亲密的“家人”）。

## 2.0 Alignment
**[2]** Korula N, Lattanzi S. "**An efficient reconciliation algorithm for social networks[J]**." Proceedings of the Vldb Endowment, 2013, 7(5):377-388. [[pdf]](https://core.ac.uk/download/pdf/24945506.pdf) :star::star:


>这篇文章提出了一个算法，将两个不同的社交网络（如Facebook 和推特）上同一个人的账号进行匹配。
>该算法首先需要一个种子集合，该集合中包含少量已经匹配好的顶点。然后，通过计算相似度（类似于simrank的方法）来找到其他两两匹配的顶点。
## 3.0 Coloring
**[3]** Peng Y, Choi B, He B, et al. "**VColor: A practical vertex-cut based approach for coloring large graphs[C]**."IEEE, International Conference on Data Engineering. IEEE, 2016:97-108.[[pdf]](http://xueshu.baidu.com/s?wd=paperuri%3A%28083cf29d6957993fd7b377ae77d2beab%29&filter=sc_long_sign&tn=SE_xueshusource_2kduw22v&sc_vurl=http%3A%2F%2Fieeexplore.ieee.org%2Fxpls%2Fabs_all.jsp%3Farnumber%3D7498232&ie=utf-8&sc_us=8490760281829948632) :star:

>这篇文章提出了一种基于顶点分割的图着色方法，这种方法将图切分成较小的子图，通过对子图分别着色再合并从而对整个图进行着色。
>这篇文章还提出了对图数据库（一系列有关联的图）进行批量着色的方法，该方法比每个图分别着色性能有显著提高。


## 4.0 Visualize
**[4]** Yan N, Hasani S, Asudeh A, et al.**Generating Preview Tables for Entity Graphs[C]**". International Conference, 2014:1797-1811.[[pdf]](https://core.ac.uk/download/pdf/25011990.pdf) :star:

>在图数据较大时，为了能够快速直观的了解一个图的属性及其内容，可以通过生成该图的“preview table”。实体图是顶点分为不同类别的图，这篇文章提出的算法通过找到“key attributes”，对每个“key attributes”生成一个table，该table 中包含对应的“key attributes”及与这个“key attributes”有“relationship”的其他属性（在多个候选中选择比较重要的）。最后再选取几个实例作为这个table的内容。

## 5.0 Parallel
**[5]** Wang Z, Gu Y, Bao Y, et al. " **Hybrid Pulling/Pushing for I/O-Efficient Distributed and Iterative Graph Computing[C]**". International Conference, 2016:479-494.[[pdf]](http://dl.acm.org/citation.cfm?id=2882938) :star::star::star:

>在分布式迭代式图计算中，有两种进行数据交换的方式，pull方式和push方式。这两种方式分别有其优缺点。这篇文章提出了一个“hybrid”的方法，通过在迭代时不同算法具有的特性而动态地调整所使用的方法，从而使IO更有效率。
## 6.0 Ordering
**[6]** Wei H, Yu J X, Lu C, et al."** Speedup Graph Processing by Graph Ordering[C]**". International Conference, 2016:1813-1828.[[pdf]](http://www1.se.cuhk.edu.hk/~hwei/paper/sigmod16-graphorder.pdf) :star::star::star:

>这篇文章通过给图的每个顶点进行排序，以控制顶点进入内存的顺序，从而使得计算时需要密集访问的顶点能够同时被加载进入内存，从而提高计算速度。

## 7.0 Subgraph mining

**[29]** Lin X, Lin X, Lin X, et al. “**When engagement meets similarity: efficient (k,r)-core computation on social networks[J]**". Proceedings of the Vldb Endowment, 2017, 10(10):998-1009.[[pdf]](http://www.vldb.org/pvldb/vol10/p998-zhang.pdf) :star::star::star:

>在社交网络上，（k，r）核是指在好友关系网络中是k核，在好友相似度网络中是clique的子图。r是相似度阈值。作者提出了若干个枚举算法来进行计算。


**[7]** Arora A, Sachan M, Bhattacharya A. “**Mining statistically significant connected subgraphs in vertex labeled graphs[C]**". ACM SIGMOD International Conference on Management of Data. ACM, 2014:1003-1014.[[pdf]](https://www.researchgate.net/publication/266656404_Mining_statistically_significant_connected_subgraphs_in_vertex_labeled_graphs) :star::star::star:

>与挖掘频繁子图类似，挖掘统计学显著子图是找出图中显著偏离预期（零假设）的子图。关联规则挖掘是统计学显著子图挖掘的一个应用。本文通过关联规则挖掘来详细描述了相关算法。

**[8]** Ruchansky N, Bonchi F, Garc, et al. "**The Minimum Wiener Connector Problem[C]**". ACM SIGMOD International Conference on Management of Data. ACM, 2015:1587-1602.[[pdf]](https://www.researchgate.net/publication/274427137_The_Minimum_Wiener_Connector_Problem) :star::star::star:

>一个图的Wiener index是一个图上所有（一对顶点之间的）最短距离之和。这篇文章研究了新的问题——找到一个图的极小Wiener connector：给定一个连图G = (V; E)，以及一个点集Q ⊆ V，找到一个G的子图，它使得Q中的所有点连通，并有着最小的Wiener index。该问题是一个NP-hard问题，作者找出了一个近似算法。

**[9]** Berlowitz D, Cohen S, Kimelfeld B. "**Efficient Enumeration of Maximal k-Plexes[C]**". ACM SIGMOD International Conference. ACM, 2015:431-444.[[pdf]](http://dl.acm.org/citation.cfm?id=2749449) :star::star::star::star:

>在图中寻找所有的极大cliques问题是一个非常重要的问题。然而在现实生活中，cliques的条件过于苛刻了。k-plex是cliques的一种变种，指的是在一个cliques中，允许每个顶点最多可以“失去”k个邻居。这篇文章提出了一个高效的算法来枚举图中的所有极大k-plex，以及“连通的”极大k-plex。当k是一个常数时，该算法有多项式时间的延迟。

**[10]** Shao Y, Chen L, Cui B. "**Efficient cohesive subgraphs detection in parallel[C]**". ACM SIGMOD International Conference on Management of Data. ACM, 2014:613-624.[[pdf]](http://net.pku.edu.cn/~cuibin/Papers/2014-SIGMOD_CohensiveSubgraph.pdf) :star::star:

>已有的并行识别k-truss的算法在大图上都效率低下，在这篇文章中，作者提出了一个新的高效的k-truss发现算法，叫做PETA。PETA在每个计算节点上生成一个完全三角子图（TC-subgraph），借助完全三角子图，PETA可以在很少的迭代次数下就发现本地的k-truss，而通信开销被固定在三角形数目的三倍以内。

**[11]** Gurukar S, Ranu S, Ravindran B. "**COMMIT: A Scalable Approach to Mining Communication Motifs from Dynamic Networks[J]**". ACM SIGMOD International Conference. ACM,, 2015:475-489.[[pdf]](http://space.cse.iitm.ac.in/~ravi/papers/Saket_thesis.pdf) :star::star::star::star:

>在这篇文章中，作者研究从动态社交网络中挖掘Communication motifs的问题。动态社交网络中每个点代表一个个体，每条边上标注了这条边（代表着两个节点之间的交互信息）的产生时间。Motif是一个子图，该子图表示了一种信息传递的模式。由于枚举子图的时间消耗较大，作者提出了一个算法COMMIT，该算法能够将图转化成一个序列，枚举子图就可以转化为找特定的子序列的问题。再将找出的子序列转化为子图。这样能够大大缩短时间。

**[12]** Chen P L, Chou C K, Chen M S. "**Distributed algorithms for k-truss decomposition[C]**". IEEE International Conference on Big Data. IEEE, 2014:471-480.[[pdf]](http://ieeexplore.ieee.org/document/7004264/?arnumber=7004264) :star::star::star:

>k-truss是一个每条边都被包含在至少K-2个三角形中的子图。给定一个图G，k-truss分解就是找到所有的k-truss。该问题可以转换为找出每条边最多被几个三角形包含的问题。作者提出了一个基于pergel的以点为中心的模型的迭代算法。

**[13]** Wu Y, Jin R, Zhu X, et al. "**Finding dense and connected subgraphs in dual networks[C]**". IEEE, International Conference on Data Engineering. IEEE, 2015:915-926.[[pdf]](https://faculty.ist.psu.edu/xzz89/publications/DCS_ICDE15.pdf) :star::star::star::star:

>对于一个dual network（包含两个图，概念图和物理图），如何找到在概念图中密度大而在物理图中联通的子图？作者提供了一个多项式的近似算法来解决这个问题。

**[14]** Batagelj V, Zaveršnik M. "**Fast algorithms for determining (generalized) core groups in social networks[J]**". Advances in Data Analysis and Classification, 2011, 5(2):129-145.[[pdf]](https://link.springer.com/article/10.1007/s11634-010-0079-y):star::star::star::star::star:


>本文介绍了k-core的概念，算法（线性）以及提出了一个k-core的扩展（g-core，通过设计不同的条件函数），以及g-core的算法。

**[15]** Li R H, Qin L, Yu J X, et al. "**Influential community search in large networks[J]**". Proceedings of the Vldb Endowment, 2015, 8(5):509-520.[[pdf]](http://www.vldb.org/pvldb/vol8/p509-li.pdf):star::star::star:


>这篇文章介绍了如何在大图中查找top-k个“影响力最大”的k-core（影响力是按这个k-core中影响力最低的那个节点作为这个k-core的影响力）。作者提出了线性的算法来寻找这样的k-core，同时设计了一种树形索引来存放这些k-core，使计算过程更加优化。

**[16]** Wen D, Qin L, Zhang Y, et al. "**I/O efficient Core Graph Decomposition at web scale[C]**". IEEE, International Conference on Data Engineering. IEEE, 2015:133-144.[[pdf]](http://de.arxiv.org/pdf/1511.00367):star::star::star:

>这篇文章提出了在硬盘上进行k-core计算的新算法。该算法和内存算法不同，由于硬盘的读写是顺序的，该算法利用了这个特性，从而使计算过程十分迅速。同时，作者还提供了在图发生变化的时候，例如增加和删除边的时候，对k-core的更新，该方法可以只更新那些受到改变的点，而不需要更新整个图，使计算速度大大提高了。


## 8.0 Keyword search


**[28]** Zhu R, Zou Z, Li J. "**Diversified Coherent Core Search on Multi-Layer Graphs[J]**". CoRR, abs/1709.09471.[[pdf]](https://arxiv.org/pdf/1709.09471.pdf):star::star:
  
>这篇文章介绍了在多层网络中，如何找到既具有多样性（包含的相同顶点少），一致性（在若干层网络中都是core）的多个子图。该文章提出了三个方法，top-down, bottom-up和混合方法。

**[17]** Jiang M, Fu W C, Wong C W. "**Exact Top-k Nearest Keyword Search in Large Networks[C]**". ACM SIGMOD International Conference. ACM, 2015:393-404.[[pdf]](http://home.cse.ust.hk/~raywong/paper/sigmod15-topKKeywordSearch.pdf):star::star::star:


>这篇文章介绍了如何在大规模图中找到距离某个顶点最近的k个包含给定关键词的顶点的搜索方法。本文通过建立两层索引，大规模的减少了搜索的过程。

## 9.0 Spanning tree
**[18]** Huang S, Fu W C, Liu R."**Minimum Spanning Trees in Temporal Graphs[C]**". ACM SIGMOD International Conference. ACM, 2015:419-430.[[pdf]](http://www.cs.cuhk.hk/~adafu/Pub/MST-sigmod2015.pdf):star::star:

>最小生成树的计算是一类非常基础的图计算问题，然而，在动态图上的最小生成树问题却很少有研究。这篇文章定义了两类最小生成树问题，分别是最小时间和最小开销。对于最小时间的最小生成树问题，作者提出了一个线性时间算法，而对于最小开销的最小生成树问题，作者提出了一个近似算法。

## 10.0 Influence maximazation 
**[19]** Li H, Bhowmick S S, Cui J, et al. "**GetReal: Towards Realistic Selection of Influence Maximization Strategies in Competitive Networks[C]**". ACM SIGMOD International Conference on Management of Data. ACM, 2015:1525-1537.[[pdf]](http://www.cais.ntu.edu.sg/~assourav/papers/SIGMOD-15-GetReal.pdf):star::star:

>这篇文章介绍了在有多个集团进行竞争的时候，如何在社交网络中选择节点进行产品推广，使产品的影响力（知晓的人数）最大。这篇文章提出了基于现实的假设，采用博弈论的原理，设计了一种多种策略混合的混合方法，使各方达到多赢（纳什均衡）。




## 11.0 Random walk
**[20]** Shin K, Jung J, Lee S, et al. "**BEAR:Block Elimination Approach for Random Walk with Restart on Large Graphs[C]**". ACM SIGMOD International Conference. ACM, 2015:1571-1585.[[pdf]](http://www.cs.cmu.edu/~kijungs/papers/bearSIGMOD2015poster.pdf):star:

>Random walk with restart是一类非常重要的问题。然而，大多数Random walk with restart的计算都是基于邻接矩阵的。在大图上，使用邻接矩阵是不高效的。在这篇文章中，作者提出了BEAR来高效地计算Random walk with restart。BEAR将图的邻接矩阵重新排序，使邻接矩阵形成块对角矩阵，和较为稠密的其他部分。这样，便于将块对角矩阵进行LU分解，从而降低计算的复杂性。

## 12.0 Road network 
**[21]** Chen Z, Liu Y, Wong C W, et al. "**Efficient algorithms for optimal location queries in road networks[C]**". ACM SIGMOD International Conference on Management of Data. ACM, 2014:123-134.[[pdf]](http://www.cse.ust.hk/~raywong/paper/sigmod14-olq.pdf):star:

>这是一篇关于道路网的文章。在这篇文章中，作者研究了基于道路网的最佳方位查询问题。即，找到一个位置来放置一个server，使得（加上这个新放置的server后）所有servers服务的clients的最大开销最小化。

## 13.0 Anomaly and significance detection 
**[22]** Noble C C, Cook D J. "**Graph-based anomaly detection[C]**". ACM SIGKDD International Conference on Knowledge Discovery and Data Mining, Washington, Dc, Usa, August. DBLP, 2003:631-636.[[pdf]](https://www.researchgate.net/publication/221653954_Graph-based_anomaly_detection):star::star:

>这篇文章介绍了两种图异常发现的方法。第一种是在一张图中找到异常的子图，第二种方法是给出许多图，在这些图中找到最异常的一个。两种方法均是基于频繁子图挖掘的假设——“模式”是频繁发生的，而“异常”是不频繁发生的，因此异常发现可以看做是找最不频繁发生的子图的问题。

**[23]** Hooi B, Song H A, Beutel A, et al. "**FRAUDAR:Bounding Graph Fraud in the Face of Camouflage[C]**" . ACM SIGKDD International Conference. ACM, 2016:895-904.[[pdf]](http://alexbeutel.com/papers/kdd2016_fraudar.pdf):star::star::star::star:

>这篇文章提出了一个系统FRAUDER来找出一个二分图中，参与欺诈行为（比如，在社交网络中，让很多僵尸账号关注自己以提高自己的排名）的节点（包括欺诈点和僵尸节点）。算法并不复杂，主要是通过给每个顶点和边赋予一个“可疑度”来评估一个子图的可疑程度。然后用一个贪心算法+优先树来不断地删除可疑度较小的节点，然后计算剩下点构成子图的可疑度，最终找出可疑度最大的子图。

## 14.0 Subgraph query
**[24]** Wu Y, Yang S, Yan X. "**Ontology-based subgraph querying[C]**".  IEEE, International Conference on Data Engineering. IEEE, 2013:697-708.[[pdf]](http://cs.ucsb.edu/~xyan/papers/icde13_ontology.pdf):star::star::star::star:

>这篇文章介绍了基于“本体图”的子图查询过程。一个本体图是一个描述不同节点之间关系的图，例如描述两个节点之间的距离。在本文中，作者通过本体图中两个地点之间的距离计算两个节点之间的相似度（距离越近越相似），因为作者不想单纯的进行子图的匹配，而是进行语义上的近似查找。先通过删除一些不会出现在结果集中的顶点来缩小搜索范围，然后再在这个缩小后的图中，找到与query子图最接近的k个子图。

**[25]** He H, Singh A K. "**Graphs-at-a-time:query language and access methods for graph databases[C]**". ACM SIGMOD International Conference on Management of Data, SIGMOD 2008, Vancouver, Bc, Canada, June. DBLP, 2010:405-418.[[pdf]](http://sites.fas.harvard.edu/~cs265/papers/he-2008.pdf):star::star:

>这篇文章提出了一个系统“Graphs-at-a-time”，该系统可以接受用户类似于SQL语句的对子图query问题的描述，然后进行子图查询。优点是用户的交互性好，同时，可以支持多种多样的query条件

**[26]** Yang S, Han F, Wu Y, et al. "**Fast top-k search in knowledge graphs[C]**".IEEE, International Conference on Data Engineering. IEEE, 2016:990-1001.[[pdf]](http://eecs.wsu.edu/~yinghui/mat/papers/star_tree-ICDE16.pdf):star:

>这篇文章提出了不同于通常的“阈值算法”的新框架STAR来进行子图的query计算。该框架执行star query非常迅速，对于一般的query，该框架可以将其分解成多个star query，并在之后将它们join起来。在分解一般的query的过程中，该文章使用了机器学习的方法来优化。

## 15.0 Recommendation
**[27]** Koren Y. "**Factorization meets the neighborhood: a multifaceted collaborative filtering model[C]**".  ACM SIGKDD International Conference on Knowledge Discovery and Data Mining. ACM, 2008:426-434. [[pdf]](http://www.inf.ed.ac.uk/teaching/courses/dme/studpres0910/DME-presentation-final.pdf):star::star::star::

>这篇文章介绍了协同过滤，引进了“隐式信息”，分别提出了新的基于邻居的模型和基于潜在因子的模型，并结合了两种模型，提出了一个新的精确度更高的模型。这是第一次一个单一的模型整合了两种方法


## Recent work

