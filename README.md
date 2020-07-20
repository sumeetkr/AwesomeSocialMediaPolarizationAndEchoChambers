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


2018, Lahoti, Preethi, Kiran Garimella, and Aristides Gionis. "Joint non-negative matrix factorization for learning ideological leaning on Twitter." In Proceedings of the Eleventh ACM International Conference on Web Search and Data Mining, pp. 351-359. ACM, 2018. https://arxiv.org/pdf/1711.10251.pdf 

2018, Stewart, Leo G., Ahmer Arif, and Kate Starbird. ["Examining trolls and polarization with a retweet network." In Proc. ACM WSDM, Workshop on Misinformation and Misbehavior Mining on the Web (to appear). Accessed January. 2018.](http://faculty.washington.edu/kstarbi/examining-trolls-polarization.pdf)

2018, Nabeel Gillani, Ann Yuan, Martin Saveski, Soroush Vosoughi, and Deb Roy. 2018. Me, My Echo Chamber, and I: Introspection on Social Media Polarization. In Proceedings of the 2018 World Wide Web Conference (WWW '18). International World Wide Web Conferences Steering Committee, Republic and Canton of Geneva, Switzerland, 823-831. DOI: https://doi.org/10.1145/3178876.3186130

2018, Kiran Garimella et al. [Political Discourse on Social Media: Echo Chambers, Gatekeepers, and the Price of Bipartisanship](https://arxiv.org/pdf/1801.01665.pdf)

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

2017, M. T. A. Amin, C. Aggarwal, S. Yao, T. Abdelzaher and L. Kaplan, "Unveiling polarization in social networks: A matrix factorization approach," IEEE INFOCOM 2017 - IEEE Conference on Computer Communications, Atlanta, GA, 2017, pp. 1-9.
doi: 10.1109/INFOCOM.2017.8056959

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

