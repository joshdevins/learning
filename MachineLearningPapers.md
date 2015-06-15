# Machine Learing Papers

## Large-Scale Supervised Learning

* [A Stochastic Gradient Method with an Exponential Convergence Rate for Strongly-Convex Optimization with Finite Training Sets](http://hal.inria.fr/docs/00/71/50/15/PDF/sag_arxiv.pdf). Nicolas Le Roux, Mark Schmidt, and Francis Bach. Tech. Report, 2012.
> Review of several stochastic gradient methods for optimizing the sum of a finite set of smooth functions.

* [A Stochastic Gradient Method with an Exponential Convergence  Rate for Finite Training Sets](http://books.nips.cc/papers/files/nips25/NIPS2012_1246.pdf). Nicolas Le Roux, Mark Schmidt, and Francis Bach. NIPS, 2012.
> Conference version of the above paper.

* [Large-Scale Support Vector Machines: Algorithms and Theory](http://cseweb.ucsd.edu/~akmenon/ResearchExam.pdf). Aditya K. Menon. Tech. Report, 2010.
> Survey on large-scale SVMs.

* [Feature Hashing for Large Scale Multitask Learning](http://arxiv.org/pdf/0902.2206). Kilian Weinberger, Anirban Dasgupta, John Langford, Alex Smola, and Josh Attenberg. ICML, 2009.
> Presents a way on how to build user-specific features, to reduce the effective number of features, and to train a single model which can be decomposed into a joint (global) model and a per-user section.

* [Sparse Multinomial Logistic Regression via Bayesian L1 Regularisation](http://books.nips.cc/papers/files/nips19/NIPS2006_0216.pdf). Gavin C. Cawley, Nicola L. C. Talbot, Mark Girolami. NIPS, 2006.
> Multinomial logistic regression provides the standard penalised maximum-likelihood solution to multi-class pattern recognition problems. This paper paper proposes a sparse multinomial logistic regression method, in which the sparsity arises from the use of a Laplace prior, but where the usual regularisation parameter is integrated out analytically.

## Metric Learning and Similarity Search

* [Similarity Search in High Dimensions Via Hashing](http://www.bradblock.com.s3-website-us-west-1.amazonaws.com/Similarity_Search_in_High_Dimensions_via_Hashing.pdf). Aristides Gionis, Piotr Indyky, and Rajeev Motwaniz. VLDB, 1999.
> One of the first papers on LSH.

* [Angular Quantization-based Binary Codes for Fast Similarity Search](http://books.nips.cc/papers/files/nips25/NIPS2012_0584.pdf). Yunchao Gong, Sanjiv Kumar, Vishal Verma, and Svetlana Lazebnik. NIPS, 2012.
> This paper focuses on the problem of learning binary embeddings for efficient retrieval of high-dimensional non-negative data. Such data typically arises in a large number of vision and text applications where counts or frequencies are used as features.

* [A Geometric take on Metric Learning](http://books.nips.cc/papers/files/nips25/NIPS2012_0997.pdf). Søren Hauberg, Oren Freifeld, and Michael J. Black. NIPS, 2012.


## Graph-based Learning

* [Authority Rankings from HITS, PageRank, and Salsa: Existence, Uniqueness, and effect of Initialization](http://www.math.hmc.edu/~ward/paperpdfs/hitsheaderbw6Jan05.pdf). Ayman Farahat, Thomas Lofaro, Joel C. Miller, Gregory Rae, and Lesley A. Ward. Tech. Report, 2005.
> Good survey on link analysis methods for ranking.

* [Combating Web Spam with TrustRank](http://www.vldb.org/conf/2004/RS15P3.PDF). Zoltán Gyöngyi, Hector Garcia-Molina, and Jan Pedersen. Proceedings of the International Conference on Very Large Data Bases, 2004.
> As BadRank/SpamRank propagates spamminess, TrustRank exploits the social graph to propagate reputation across the nodes (users).

* [DirichletRank: Solving the Zero-One Gap Problem of PageRank](http://research.microsoft.com/apps/pubs/default.aspx?id=79479) - [PDF](http://www.xuanhui.me/pub/drank.pdf). ACM Transactions on Information Systems (TOIS), Volume 26 Issue 2, March 2008.
> + PageRank algorithm solving the "dangling nodes" problem
> + PageRank variant (DirichletRank) which produces a smooth transition probability based on the number of outgoing edges, preventing spammers from taking advantage of the change in transition probability from, e.g., 0 outgoing edges to 1.

* [WTF: The Who to Follow Service at Twitter](http://www.stanford.edu/~rezab/papers/wtf_overview.pdf). Pankaj Gupta, Ashish Goel, Jimmy Lin, Aneesh Sharma, Dong Wang, Reza Zadeh. Proceedings of the 22th International World Wide Web Conference (WWW 2013), May 2013, Rio de Janeiro, Brazil.

* [Topic-Sensitive PageRank](http://dl.acm.org/citation.cfm?id=511513) [pdf](http://ilpubs.stanford.edu:8090/573/1/2002-6.pdf). Taher H. Haveliwala. Proceedings of the 11th International World Wide Web Conference (WWW 2002), May 2002, Budapest, Hungary.
> In the original PageRank algorithm for improving the ranking of search-query results, a single PageRank vector is computed, using the link structure of the Web, to capture the relative "importance" of Web pages, independent of any particular search query. To yield more accurate search results, we propose computing a set of PageRank vectors, biased using a set of representative topics, to capture more accurately the notion of importance with respect to a particular topic. By using these (precomputed) biased PageRank vectors to generate query-specific importance scores for pages at query time, we show that we can generate more accurate rankings than with a single, generic PageRank vector. For ordinary keyword search queries, we compute the topic-sensitive PageRank scores for pages satisfying the query using the topic of the query keywords. For searches done in context (e.g., when the search query is performed by highlighting words in a Web page), we compute the topic-sensitive PageRank scores using the topic of the context in which the query appeared.

## Content-based & Collaborative Filtering

* [A Survey of Collaborative Filtering Techniques](http://www.hindawi.com/journals/aai/2009/421425/). Xiaoyuan Su and Taghi M. Khoshgoftaar. Advances in Artificial Intelligence, 2009.
> Not complete but nice to read survey on collaborative filtering methods. The paper first introduce CF tasks and their main challenges, such as data sparsity, scalability, synonymy, gray sheep, shilling attacks, privacy protection, etc., and their possible solutions. Then, three main categories of CF techniques are discussed: memory-based, model-based, and hybrid CF algorithms with examples for representative algorithms of each category, and analysis of their predictive performance and their ability to address the challenges. From basic techniques to the state-of-the-art, the paper presents a comprehensive survey for CF techniques which can be served as a roadmap for research and practice in this area.

* [Matchbox: Large Scale Online Bayesian Recommendations](http://research.microsoft.com/pubs/79460/www09.pdf). David Stern, Ralf Herbrich, and Thore Graepel. WWW, 2009.
> This paper presents a Bayesian method that naturally extends matrix-factorization concepts to content-based filtering. The method can be used for distributed real-time recommendation and makes use of user as well as item information. It is based on approximate message passing and expectation propagation. It is used in Microsoft's XBox; and Facebook has a working prototype for recommending feeds. However, the underlying theory and the implementation is far from trivial!

* [Collaborative Ranking with 17 Parameters](http://books.nips.cc/papers/files/nips25/NIPS2012_1122.pdf). Maksims Volkovs and Richard Zemel. NIPS, 2012.
> Nice approach that translates the recommendation problem into a supervised ranking problem. It is simple but powerful; however, needs tweeking to scale it.

* [CofiRank - Maximum Margin Matrix Factorization for Collaborative Ranking](http://books.nips.cc/papers/files/nips20/NIPS2007_0612.pdf). Markus Weimer, Alexandros Karatzoglou, Quoc Viet Le, and Alex Smola. NIPS, 2007.
> One of the first collaborative filtering methods that do not focus on predicting the numerical score/rating but the correct order w.r.t. relevancy. As a by-product, the authors develop a new method for supervised ranking by minimizing an upper bound on the NDCG loss.

* [Improving Maximum Margin Matrix Factorization](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.140.4647&rep=rep1&type=pdf). Markus Weimer, Alexandros Karatzoglou, and Alex Smola. ECML/PKDD, 2008.
> Presents some general ideas on how to improve matrix factorization-based collaborative filtering, e.g., feature normalization, dealing with regularization, user & item-bias etc.

* [Collaborative Filtering for Implicit Feedback Datasets](http://www2.research.att.com/~yifanhu/PUB/cf.pdf). Y. Hu, Y. Koren, and C. Volinsky. ICDM, 2008.
> Unlike the much more extensively researched "explicit" feedback, this paper deals with the problem of not having any direct input from the users regarding their preferences; in particular, tasks with a lack of evidence on which products consumer dislike. This work identifies unique properties of implicit feedback datasets and proposes to treat the data as indication of positive and negative preference associated with vastly varying confidence levels. This leads to a factor model which is especially tailored for implicit feedback recommenders.

* [Comparison of Collaborative Filtering Algorithms: Limitations of Current Techniques and Proposals for Scalable, High-Performance Recommender Systems](http://www.stlab.istc.cnr.it/documents/papers/aemoo/15%20-%20Cacheda%20et%20al%20-%202011.pdf). Fidel Cacheda, Victor Carneiro, Diego Fernández, and Vreixo Formoso. TWEB, 2011.
> This paper discusses the problem of evaluating collaborative filtering algorithms. The authors compare different techniques found in the literature, and study the characteristics of each one, highlighting their principal strengths and weaknesses. Several experiments are performed using the most popular metrics and algorithms. Moreover, two new metrics are presented to measure the precision on good items.

* [Google News Personalization: Scalable Online Collaborative Filtering](http://www2007.org/papers/paper570.pdf). Abhinandan S. Das, Mayur Datar, Ashutosh Garg, and Shyam Rajaram. WWW, 2007.
> This paper describes Google's approach to collaborative filtering for generating personalized recommendations for users of Google News. Recommendations are genereated using three approaches: collaborative filtering using MinHash clustering, Probabilistic Latent Semantic Indexing (PLSI), and covisitation counts. Recommendations from different algorithms are combined using a linear model. The approach is content agnostic and consequently domain independent, making it easily adaptable for other applications and languages with minimal effort.

* [Large-scale Parallel Collaborative Filtering for the Netﬂix Prize](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.173.2797&rep=rep1&type=pdf). Yunhong Zhou, Dennis Wilkinson, Robert Schreiber and Rong Pan. Lecture Notes in Computer Science Volume 5034, 2008.
> Two major problems that most CF approaches have to contend with are scalability and sparseness of the user profiles. To tackle these issues, the authors describe a CF algorithm alternating-least-squares with weighted-lambda-regularization (ALS-WR).

* [Collaborative Filtering on a Budget](http://jmlr.csail.mit.edu/proceedings/papers/v9/karatzoglou10a/karatzoglou10a.pdf). Alexandros Karatzoglou, Alex Smola and Markus Weimer. Journal of Machine Learning Research, 2010.
>  In this paper, we propose a new model for representing and compressing matrix factors via hashing. This allows for essentially unbounded storage (at a graceful storage/performance trade-off) for users and items to be represented in a pre-defined memory footprint.  It allows us to scale recommender systems to very large numbers of users or conversely, obtain very good performance even for tiny models (e.g. 400kB of data suffice for a representation of the EachMovie problem).

* [One-Class Collaborative Filtering](http://www.hpl.hp.com/techreports/2008/HPL-2008-48R1.pdf). Rong Pan, Yunhong Zhou, Bin Cao, Nathan N. Liu, Rajan Lukose, Martin Scholz, and Qiang Yang. ECML/PKDD, 2008.

* [Scalable Similarity-Based Neighborhood Methods
with MapReduce](http://ssc.io/wp-content/uploads/2012/06/rec11-schelter.pdf). Sebastian Schelter, Christoph Boden, and Volker Markl. RecSys, 2011.
> Similarity-based neighborhood methods, a simple and popular approach to collaborative filtering, infer their predictions by finding users with similar taste or items that have been similarly rated. If the number of users grows to millions, the standard approach of sequentially examining each item and looking at all interacting users does not scale.

* [The BellKor Solution to the Netflix Grand Prize](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.162.2118&rep=rep1&type=pdf). Yehuda Koren. 2009.
> This article describes part of our contribution to the "Bell-Kor's Pragmatic Chaos" final solution, which won the Netflix Grand Prize. The other portion of the contribution was created while working at AT&T with Robert Bell and Chris Volinsky, as reported in our 2008 Progress Prize report. The final solution includes all the predictors described there. In this article we describe only the newer predictors.

* [Collaborative Filtering with Temporal Dynamics](http://research.yahoo.com/files/kdd-fp074-koren.pdf). Yehuda Koren. KDD '09 Proceedings of the 15th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining. Pages 447-456. ACM, 2009.
> Customer preferences for products are drifting over time. Product perception and popularity are constantly changing as new selection emerges. Similarly, customer inclinations are evolving, leading them to ever redefine their taste. Thus, modeling temporal dynamics should be a key when designing recommender systems or general customer preference models.

* [Recommendation over a Heterogeneous Social Network](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.141.2561). Jing Zhang, Jie Tang, Bangyong Liang, Zi Yang, Sijie Wang, Jingjing Zuo, Juanzi Li, 2007.
  * looks at the problem of ranking on a network made of users, items, categories, etc.  
  * was found in a [presentation](http://www.slideshare.net/clickstone/social-recommendation) that in itself is quite interesting

## Music Classification & Recommendation

* [Hypergraph Models of Playlist Dialects](http://cseweb.ucsd.edu/~bmcfee/papers/ismir2012_dialect.pdf). Brian McFee and Gert Lanckriet. ISMIR, 2012.
> Playlist generation is an important task in music information retrieval. While previous work has treated a playlist collection as an undifferentiated whole, the authors of this paper propose to build playlist models which are tuned to specific categories or dialects of playlists. Toward this end, they develop a general class of flexible and scalable playlist models based upon hypergraph random walks. [Code](https://github.com/bmcfee/hypergraph_playlist)

* [A Survey of Music Recommendation Systems and Future Perspectives](http://cmmr2012.eecs.qmul.ac.uk/sites/cmmr2012.eecs.qmul.ac.uk/files/pdf/papers/cmmr2012_submission_42.pdf). Yading Song, Simon Dixon, and Marcus Pearce. CMMR, 2012.

* [A Preliminary Study on a Recommender System for the
Million Songs Dataset Challenge](http://www.math.unipd.it/~aiolli/PAPERS/MSDaiolli.pdf) Fabio Aiolli. Kaggle Million Song Dataset challenge, 2010. [Kaggle challenge](http://www.kaggle.com/c/msdchallenge).
> In this paper the preliminary study we are conducting on the Million Songs Dataset (MSD) challenge is described. The task of the competition is to suggest a set of songs to a user given half of its listening history and complete listening history of other 1 million people.

* [GMM Supervector For Content Based Music Similarity](http://recherche.ircam.fr/pub/dafx11/Papers/98_e.pdf) Christophe Charbuillet, Damien Tardieu and Geoffroy Peeters. IRCAM-STMS-CNRS, Centre Pompidou, 2011
>Timbral modeling is fundamental in content based music similarity systems. It is usually achieved by modeling the short term features by a Gaussian Model (GM) or Gaussian Mixture Models (GMM).

* [Block-Level Audio Features for Music Genre Classification](http://www.cp.jku.at/people/schedl/Research/Publications/pdf/ss_gc_mirex_2009.pdf) Klaus Seyerlehner, Markus Schedl, MIREX 2010
> While frame-level audio features, e.g. MFCCs, in combination with the bag-of-frames approach have widely and successfully been used, we use a block processing framework in our submission. In general block-level features have the advantage that they can capture more temporal information than BOF approaches can. We introduce two novel spectral patterns, closely related to the  spectrum histogram and propose a modified version of the well-known fluctuation patterns.

* [Improving Automatic Music Tag Annotation Using Stacked Generalization Of Probabilistic SVM Outputs](http://webhome.cs.uvic.ca/~gtzan/work/pubs/acm2009gtzan.pdf) S. R. Ness, A. Theocharis,
G. Tzanetakis, L. G. Martins, 17th ACM Int. Conf. on Multimedia, 2009
> Music listeners frequently use words to describe music. Personalized music recommendation systems such as Last.fm and Pandora rely on manual annotations (tags) as a mechanism for querying and navigating large music collections. A well-known issue in such recommendation systems is known as the cold-start problem: it is not possible to recommend new songs/tracks until those songs/tracks have been manually annotated. Automatic tag annotation based on content analysis is a potential solution to this problem and has recently been gaining attention. We describe how stacked generalization can be used to improve the performance of astate-of-the art automatic tag annotation system for music based on audio content analysis and report results on two publicly available datasets.

* [Temporal Pooling And Multiscale Learning For Automatic Annotation and Ranking Of Music Audio](http://ismir2011.ismir.net/papers/PS6-13.pdf) Philippe Hamel, Simon Lemieux, Yoshua Bengio, Douglas Eck, ISMIR 2011
>This paper analyzes some of the challenges in performing automatic annotation and ranking of music audio, and proposes a few improvements. First, we motivate the use of principal component analysis on the mel scaled spectrum. Secondly, we present an analysis of the impact of the selection of pooling functions for summarization of the features over time. We show that combining several pooling functions improves the performance of the system. Finally, we introduce the idea of multiscale learning. By incorporating these ideas in our model, we obtained state-of-the-art performance on the Magnatagatune dataset.

## Ranking

* [Ranking and Suggesting Popular Items](http://research.microsoft.com/apps/pubs/default.aspx?id=78290) [pdf](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.137.1206). Milan Vojnovic, James Cruise, Dinan Gunawardena, and Peter Marbach. IEEE Trans. on Knowledge and Data Engineering, 2009.
> We consider the problem of ranking popularity of items and suggesting popular items based on user feedback.

## Personalized PageRank (for recommendation)

* [Lecture notes providing a very simple short introduction to Personalized PageRank for recommendation](http://www.stanford.edu/~ashishg/msande235/spr08_09/Lecture13.pdf) [pdf]

* [A good summary on PageRank and Personalised PageRank](http://pagerank.suchmaschinen-doktor.de/index/modifications.html) [website]

* Initial mention of the Personalized PageRank was in: [The PageRank Citation Ranking: Bringing Order to the Web](http://ilpubs.stanford.edu:8090/422/1/1999-66.pdf). Lawrence Page, Sergey Brin, Rajeev Motwani, Terry Winograd, 1999.
At that stage it was a very naïve idea though since it required to compute separately each personalised vector for each user and this does not scale.

* A more scalable version of the personalized PageRank can be found in [Topic-Sensitive PageRank](http://ilpubs.stanford.edu:8090/573/1/2002-6.pdf) [pdf]. Haveliwala, Taher H. In Eleventh International World Wide Web Conference (WWW 2002), 2002.
Notice that this only covers the case of personalised search results.

* An interesting paper using a personalized PageRank-like approach for recommendation (with good equations in section 3 summarizing very well how to go from general PageRank equations to equations one can use for recommendation): [ItemRank: A Random-Walk Based Scoring Algorithm for Recommender Engines](http://www.aaai.org/Papers/IJCAI/2007/IJCAI07-444.pdf) [pdf] Marco Gori, Augusto Pucci. In Proceedings of the 20th international joint conference on Artifical intelligence (IJCAI), 2007.

* Another paper also using a random walk approach to the recommendation problem, and using the sparsity of the data as an advantage: [A Random Walk Method for Alleviating the Sparsity Problem in Collaborative Filtering](http://brettb.net/project/papers/2008%20A%20random%20walk%20method%20for%20alleviating%20the%20sparsity%20problem%20in%20collaborative%20filtering.pdf) [pdf] Hilmi Yildirim, Mukkai S. Krishnamoorthy. In Proceedings of the ACM conference on Recommender systems (ACM RecSys), 2008.
