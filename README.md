# Awesome Social-Media Polarization and Echo-Chambers

This page is summarizes recent research on Polarization and Echo-chambers on Social Media.
Table of content:

# a) Data repository 

## Synthetic Dataset
Polarized groups typically contain two densely connected groups with some cross-connections. This pattern can be easily modeled by Stochastic Block Models (SBMs). Note that such a netowrk structure does not gurantee polarization, but could be used as starting point. 

I have created a Jupyter [Notebook file](https://github.com/sumeetkr/AwesomeSocialMediaPolarizationAndEchoChambers/blob/master/CreateSyntheticDataset.ipynb) that demonstrates how to cretae such networks in a few lines of code. 

Next, we will add attributes to these nodes. This is aligned with the idea that polarization of a partitioned network can be explained by nodes behaviour. For example, nodes in one group wil be 'pro' some target, whereas nodes in other group will be 'anti' the same target.

We again use the same notebook to create attributed networks [Notebook file](https://github.com/sumeetkr/AwesomeSocialMediaPolarizationAndEchoChambers/blob/master/CreateSyntheticDataset.ipynb). 


Next, i will try some of the algorithms used in some of the papers listed below to find how well they on this synthetic dataset.


## Real-World Dataset

ToDo: I have some Twitter datasets that I will add here. Other possiblity is the blogs dataset used in earlier studies.


# b) Code

To create a synthetic dataset, you can use this Jupyter [Notebook file](https://github.com/sumeetkr/AwesomeSocialMediaPolarizationAndEchoChambers/blob/master/CreateSyntheticDataset.ipynb)


# c) Publications

2020, Rashed, Ammar, Mucahid Kutlu, Kareem Darwish, Tamer Elsayed, and Cansın Bayrak. "[Embeddings-Based Clustering for Target Specific Stances: The Case of a Polarized Turkey.](https://arxiv.org/pdf/2005.09649.pdf)" arXiv preprint arXiv:2005.09649 (2020). ``On June 24, 2018, Turkey conducted a highly consequential election in which the Turkish people elected their president and parliament in the first election under a new presidential system. During the election period, the Turkish people extensively shared their political opinions on Twitter. One aspect of polarization among the electorate was support for or opposition to the reelection of Recep Tayyip Erdogan. In this paper, ˘ we present an unsupervised method for target-specific stance detection in a polarized setting, specifically Turkish politics, achieving 90% precision in identifying user stances, while maintaining more than 80% recall. The method involves representing users in an embedding space using Google’s Convolutional Neural Network (CNN) based multilingual universal sentence encoder. The representations are then projected onto a lower dimensional space in a manner that reflects similarities and are consequently clustered. We show the effectiveness of our method in properly clustering users of divergent groups across multiple targets that include political figures, different groups, and parties. We perform our analysis on a large dataset of 108M Turkish election-related tweets along with the timeline tweets of 168k Turkish users, who authored 213M tweets. Given the resultant user stances, we are able to observe correlations between topics and compute topic polarization.``


2020, Gurukar, Saket, Deepak Ajwani, Sourav Dutta, Juho Lauri, Srinivasan Parthasarathy, and Alessandra Sala. "[Towards Quantifying the Distance between Opinions.](https://www.aaai.org/ojs/index.php/ICWSM/article/download/7294/7148/)" In Proceedings of the International AAAI Conference on Web and Social Media, vol. 14, pp. 229-239. 2020. `` Increasingly, critical decisions in public policy, governance, and business strategy rely on a deeper understanding of the needs and opinions of constituent members (e.g. citizens, shareholders). While it has become easier to collect a large number of opinions on a topic, there is a necessity for automated tools to help navigate the space of opinions. In such contexts understanding and quantifying the similarity between opinions is key. We find that measures based solely on text similarity or on overall sentiment often fail to effectively capture the distance between opinions. Thus, we propose a new distance measure for capturing the similarity between opinions that leverages the nuanced observation – similar opinions express similar sentiment polarity on specific relevant entities-of-interest. Specifically, in an unsupervised setting, our distance measure achieves significantly better Adjusted Rand Index scores (up to 56x) and Silhouette coefficients (up to 21x) compared to existing approaches. Similarly, in a supervised setting, our opinion distance measure achieves considerably better accuracy (up to 20% increase) compared to extant approaches that rely on text similarity, stance similarity, and sentiment similarity.``


2020, Baumann, Fabian, Philipp Lorenz-Spreen, Igor M. Sokolov, and Michele Starnini. "[Modeling echo chambers and polarization dynamics in social networks.](https://link.aps.org/pdf/10.1103/PhysRevLett.124.048301?casa_token=w8OYI48w4ocAAAAA:29eRf3xaG3fzyYNvL08I5POEGynHOM8VoNEUZp4bpKH6DhxHpuAb0B0Cz2F-d3elO6WZoxgPboK7Jg)" Physical Review Letters 124, no. 4 (2020): 048301. ``Echo chambers and opinion polarization recently quantified in several sociopolitical contexts and across
different social media raise concerns on their potential impact on the spread of misinformation and on the openness of debates. Despite increasing efforts, the dynamics leading to the emergence of these phenomena remain unclear. We propose a model that introduces the dynamics of radicalization as a reinforcing mechanism driving the evolution to extreme opinions from moderate initial conditions. Inspired by empirical findings on social interaction dynamics, we consider agents characterized by heterogeneous activities and homophily.We show that the transition between a global consensus and emerging radicalized states is mostly governed by social influence and by the controversialness of the topic discussed. Compared with empirical data of polarized debates on Twitter, the model qualitatively reproduces the observed relation between users’ engagement and opinions, as well as opinion segregation in the interaction network. Our findings shed light on the mechanisms that may lie at the core of the emergence of echo chambers and polarization in social media.``


2019, Amelkin, Victor, Petko Bogdanov, and Ambuj K. Singh. "[A distance measure for the analysis of polar opinion dynamics in social networks.](https://dl.acm.org/doi/pdf/10.1145/3332168)" ACM Transactions on Knowledge Discovery from Data (TKDD) 13, no. 4 (2019): 1-34. ``Analysis of opinion dynamics in social networks plays an important role in today’s life. For predicting users’
political preference, it is particularly important to be able to analyze the dynamics of competing polar opinions,
such as pro-Democrat vs. pro-Republican. While observing the evolution of polar opinions in a social network
over time, can we tell when the network evolved abnormally? Furthermore, can we predict how the opinions of the
users will change in the future? To answer such questions, it is insufficient to study individual user behavior,
since opinions can spread beyond users’ ego-networks. Instead, we need to consider the opinion dynamics
of all users simultaneously and capture the connection between the individuals’ behavior and the global
evolution pattern of the social network.
In this work, we introduce the Social Network Distance (SND)—a distance measure that quantifies the
likelihood of evolution of one snapshot of a social network into another snapshot under a chosen model of
polar opinion dynamics. SND has a rich semantics of a transportation problem, yet, is computable in time linear
in the number of users and, as such, is applicable to large-scale online social networks. In our experiments
with synthetic and Twitter data, we demonstrate the utility of our distance measure for anomalous event
detection. It achieves a true positive rate of 0.83, twice as high as that of alternatives. The same predictions
presented in precision-recall space show that SND retains perfect precision for recall up to 0.2. Its precision
then decreases while maintaining more than 2-fold improvement over alternatives for recall up to 0.95. When
used for opinion prediction in Twitter data, SND’s accuracy is 75.6%, which is 7.5% higher than that of the
next best method.``

2019, Kearney, Michael Wayne. "[Analyzing change in network polarization.](https://journals.sagepub.com/doi/pdf/10.1177/1461444818822813?casa_token=PM8lcoBhWDUAAAAA:VM-Qwj4imv24JNtQvAUBBiJGETUoBCzY8YskXcKqoeRCa4hAF1yxorCwqCcEWEvqiUlXN70bIf8Q)" new media & society 21, no. 6 (2019): 1380-1402 ``The growing influence of social media in an era of media fragmentation has amplified concerns of political polarization. Yet relatively few studies have analyzed polarization in user networks over time. This study therefore examines change in network polarization on Twitter during a highly contested general election. Using Twitter’s REST API, user networks of 3000 randomly selected followers of well-known partisan and entertainmentoriented accounts were recorded 17 times in the 7 months leading up to the 2016 general election. Results suggest that partisan users form highly partisan networks on Twitter, while moderate, or less engaged, users continue to mostly avoid politics.``

2018, Lahoti, Preethi, Kiran Garimella, and Aristides Gionis. "Joint non-negative matrix factorization for learning ideological leaning on Twitter." In Proceedings of the Eleventh ACM International Conference on Web Search and Data Mining, pp. 351-359. ACM, 2018. https://arxiv.org/pdf/1711.10251.pdf 

2018, Stewart, Leo G., Ahmer Arif, and Kate Starbird. ["Examining trolls and polarization with a retweet network." In Proc. ACM WSDM, Workshop on Misinformation and Misbehavior Mining on the Web (to appear). Accessed January. 2018.](http://faculty.washington.edu/kstarbi/examining-trolls-polarization.pdf)

2018, Nabeel Gillani, Ann Yuan, Martin Saveski, Soroush Vosoughi, and Deb Roy. 2018. Me, My Echo Chamber, and I: Introspection on Social Media Polarization. In Proceedings of the 2018 World Wide Web Conference (WWW '18). International World Wide Web Conferences Steering Committee, Republic and Canton of Geneva, Switzerland, 823-831. DOI: https://doi.org/10.1145/3178876.3186130

2018, Kiran Garimella et al. [Political Discourse on Social Media: Echo Chambers, Gatekeepers, and the Price of Bipartisanship](https://arxiv.org/pdf/1801.01665.pdf)

2018, Askitas, Nikolaos. "[Explaining opinion polarisation with opinion copulas.](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0183277)" PloS one 12, no. 8 (2017): e0183277. ``An empirically founded and widely established driving force in opinion dynamics is homophily
i.e. the tendency of ªbirds of a featherº to ªflock togetherº. The closer our opinions are
the more likely it is that we will interact and converge. Models using these assumptions are
called bounded confidence models (BCM) as they assume a tolerance threshold after which
interaction is unlikely. They are known to produce one or more clusters, depending on the
size of the bound, with more than one cluster being possible only in the deterministic case.
Introducing noise, as is likely to happen in a stochastic world, causes BCM to produce consensus
which leaves us with the open problem of explaining the emergence and sustainance
of opinion clusters and polarisation. We investigate the role of heterogeneous priors
in opinion formation, introduce the concept of opinion copulas, argue that it is well supported
by findings in Social Psychology and use it to show that the stochastic BCM does indeed
produce opinion clustering without the need for extra assumptions.``


2018, Garimella, Kiran, Gianmarco De Francisci Morales, Aristides Gionis, and Michael Mathioudakis. ["Quantifying Controversy on Social Media." ACM Transactions on Social Computing 1, no. 1 (2018): 3.](https://dl.acm.org/citation.cfm?id=3140565)

2018, Sîrbu, Alina, Dino Pedreschi, Fosca Giannotti, and János Kertész. "[Algorithmic bias amplifies opinion fragmentation and polarization: A bounded confidence model.](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0213246)" PloS one 14, no. 3 (2019): e0213246.

``The flow of information reaching us via the online media platforms is optimized not by the
information content or relevance but by popularity and proximity to the target. This is typically
performed in order to maximise platform usage. As a side effect, this introduces an
algorithmic bias that is believed to enhance fragmentation and polarization of the societal
debate. To study this phenomenon, we modify the well-known continuous opinion dynamics
model of bounded confidence in order to account for the algorithmic bias and investigate its
consequences. In the simplest version of the original model the pairs of discussion participants
are chosen at random and their opinions get closer to each other if they are within a
fixed tolerance level. We modify the selection rule of the discussion partners: there is an
enhanced probability to choose individuals whose opinions are already close to each other,
thus mimicking the behavior of online media which suggest interaction with similar peers.
As a result we observe: a) an increased tendency towards opinion fragmentation, which
emerges also in conditions where the original model would predict consensus, b) increased
polarisation of opinions and c) a dramatic slowing down of the speed at which the convergence
at the asymptotic state is reached, which makes the system highly unstable. Fragmentation
and polarization are augmented by a fragmented initial population.``

2017, Garimella, Venkata Rama Kiran, and Ingmar Weber. "A long-term analysis of polarization on Twitter." In Eleventh International AAAI Conference on Web and Social Media. 2017.


2017, M. T. A. Amin, C. Aggarwal, S. Yao, T. Abdelzaher and L. Kaplan, "[Unveiling polarization in social networks: A matrix factorization approach](https://www.aaai.org/ocs/index.php/ICWSM/ICWSM17/paper/download/15592/14846)," IEEE INFOCOM 2017 - IEEE Conference on Computer Communications, Atlanta, GA, 2017, pp. 1-9.
doi: 10.1109/INFOCOM.2017.8056959 ``Social media has played an important role in shaping political discourse over the last decade. It is often perceived to have increased political polarization, thanks to the scale of discussions and their public nature. Here, we try to answer whether political polarization in the US on Twitter has increased over the last eight years. We analyze a large longitudinal Twitter dataset of 679,000 users and look at signs of polarization in their (i) network - how people follow political and media accounts, (ii) tweeting behavior - whether they retweet content from both sides, and (iii) content - how partisan the hashtags they use are. Our analysis shows that online polarization has indeed increased over the past eight years and that, depending on the measure, the relative change is 10%-20%. Our study is one of very few with such a long-term perspective, encompassing two US presidential elections and two mid-term elections, providing a rare longitudinal analysis.``

2017, Peterson, Erik, Sharad Goel, and Shanto Iyengar. ["Echo Chambers and Partisan Polarization: Evidence from the 2016 Presidential Campaign." (2017).](https://pcl.stanford.edu/research/2017/peterson-echo-chambers.pdf)

2017, Takikawa, Hiroki, and Kikuko Nagayoshi. ["Political Polarization in Social Media: Analysis of the" Twitter Political Field" in Japan." arXiv preprint arXiv:1711.06752 (2017).](https://arxiv.org/pdf/1711.06752)

2017, Tang, Shiliang, Qingyun Liu, Megan McQueen, Scott Counts, Apurv Jain, Heather Zheng, and Ben Zhao. "Echo chambers in investment discussion boards." (2017). https://www.microsoft.com/en-us/research/wp-content/uploads/2017/03/investment-echo-chambers.pdf

2016, Bessi, Alessandro, Fabiana Zollo, Michela Del Vicario, Michelangelo Puliga, Antonio Scala, Guido Caldarelli, Brian Uzzi, and Walter Quattrociocchi. "[Users polarization on Facebook and Youtube.](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0159641)" PloS one 11, no. 8 (2016): e0159641.
``Users online tend to select information that support and adhere their beliefs, and to form
polarized groups sharing the same view—e.g. echo chambers. Algorithms for content promotion
may favour this phenomenon, by accounting for users preferences and thus limiting
the exposure to unsolicited contents. To shade light on this question, we perform a comparative
study on how same contents (videos) are consumed on different online social media—
i.e. Facebook and YouTube—over a sample of 12M of users. Our findings show that content
drives the emergence of echo chambers on both platforms. Moreover, we show that the
users’ commenting patterns are accurate predictors for the formation of echo-chambers``

2015, Barberá, Pablo, John T. Jost, Jonathan Nagler, Joshua A. Tucker, and Richard Bonneau. ["Tweeting from left to right: Is online political communication more than an echo chamber?." Psychological science 26, no. 10 (2015): 1531-1542.](http://journals.sagepub.com/doi/abs/10.1177/0956797615594620)

2015, Morales, A. J., Javier Borondo, Juan Carlos Losada, and Rosa M. Benito. ["Measuring political polarization: Twitter shows the two sides of Venezuela." Chaos: An Interdisciplinary Journal of Nonlinear Science 25, no. 3 (2015): 033114](https://arxiv.org/pdf/1505.04095.pdf)
            
2015, Williams, Hywel TP, James R. McMurray, Tim Kurz, and F. Hugo Lambert. ["Network analysis reveals open forums and echo chambers in social media discussions of climate change." Global Environmental Change 32 (2015): 126-138.](https://www.sciencedirect.com/science/article/pii/S0959378015000369)

2014, Akoglu, Leman. "Quantifying Political Polarity Based on Bipartite Opinion Networks." In ICWSM. 2014. http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.432.4647&rep=rep1&type=pdf

2013, Guerra, Pedro Henrique Calais, Wagner Meira Jr, Claire Cardie, and Robert Kleinberg. ["A Measure of Polarization on Social Media Networks Based on Community Boundaries." In ICWSM. 2013.(https://www.aaai.org/ocs/index.php/ICWSM/ICWSM13/paper/viewPDFInterstitial/6104Pedro/6360)

2011, Conover, Michael, Jacob Ratkiewicz, Matthew R. Francisco, Bruno Gonçalves, Filippo Menczer, and Alessandro Flammini. ["Political polarization on twitter." ICWSM 133 (2011): 89-96](http://www.aaai.org/ocs/index.php/ICWSM/ICWSM11/paper/download/2847/3275)
    
2009, Gilbert, Eric, Tony Bergstrom, and Karrie Karahalios. ["Blogs are echo chambers: Blogs are echo chambers." In System Sciences, 2009. HICSS'09. 42nd Hawaii International Conference on, pp. 1-10. IEEE, 2009.](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.211.8065&rep=rep1&type=pdf)

# d) Tutorials
Awesome tutorial by Kiran  Garimella [Orignially shared on Dropbox](https://www.dropbox.com/s/labk5uu6e2j407h/Polarization%20on%20Social%20Media.pptx?dl=0#)

# e) Rumor and Controversy
Coletto, Mauro, Kiran Garimella, Aristides Gionis, and Claudio Lucchese. "A motif-based approach for identifying controversy." arXiv preprint arXiv:1703.05053 (2017).


# f) Useful Websites
BuzzFeedNews [Partisan News Analysis](https://github.com/BuzzFeedNews/2017-08-partisan-sites-and-facebook-pages) 
BBC [The-myth-of-the-online-echo-chamber](http://www.bbc.com/future/story/20180416-the-myth-of-the-online-echo-chamber)

# g) Related Publications, but not necessarily on the topic above

