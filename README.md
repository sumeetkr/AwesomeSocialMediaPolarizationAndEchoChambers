# Awesome Social-Media Polarization and Echo-Chambers

This page is summarizes recent research on Polarization and Echo-chambers on Social Media. Unlike other survey pages, this site will focus on explaining research contibution along with data and code snippets (when possible). The page is Inspired by other 'awesome' github pages like [awesome-deep-learning](https://github.com/ChristosChristofidis/awesome-deep-learning).

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
2018, Stewart, Leo G., Ahmer Arif, and Kate Starbird. ["Examining trolls and polarization with a retweet network." In Proc. ACM WSDM, Workshop on Misinformation and Misbehavior Mining on the Web (to appear). Accessed January. 2018.](http://faculty.washington.edu/kstarbi/examining-trolls-polarization.pdf)

2018, Nabeel Gillani, Ann Yuan, Martin Saveski, Soroush Vosoughi, and Deb Roy. 2018. Me, My Echo Chamber, and I: Introspection on Social Media Polarization. In Proceedings of the 2018 World Wide Web Conference (WWW '18). International World Wide Web Conferences Steering Committee, Republic and Canton of Geneva, Switzerland, 823-831. DOI: https://doi.org/10.1145/3178876.3186130

2018, Kiran Garimella et al. [Political Discourse on Social Media: Echo Chambers, Gatekeepers, and the Price of Bipartisanship](https://arxiv.org/pdf/1801.01665.pdf)

2018, Garimella, Kiran, Gianmarco De Francisci Morales, Aristides Gionis, and Michael Mathioudakis. ["Quantifying Controversy on Social Media." ACM Transactions on Social Computing 1, no. 1 (2018): 3.](https://dl.acm.org/citation.cfm?id=3140565)

    Important Contributions:

    
    Dataset Used:

    
    Analysis:


2017, Peterson, Erik, Sharad Goel, and Shanto Iyengar. ["Echo Chambers and Partisan Polarization: Evidence from the 2016 Presidential Campaign." (2017).](https://pcl.stanford.edu/research/2017/peterson-echo-chambers.pdf)

2017, Takikawa, Hiroki, and Kikuko Nagayoshi. ["Political Polarization in Social Media: Analysis of the" Twitter Political Field" in Japan." arXiv preprint arXiv:1711.06752 (2017).](https://arxiv.org/pdf/1711.06752)

2017, Tang, Shiliang, Qingyun Liu, Megan McQueen, Scott Counts, Apurv Jain, Heather Zheng, and Ben Zhao. "Echo chambers in investment discussion boards." (2017). https://www.microsoft.com/en-us/research/wp-content/uploads/2017/03/investment-echo-chambers.pdf

2015, Barberá, Pablo, John T. Jost, Jonathan Nagler, Joshua A. Tucker, and Richard Bonneau. ["Tweeting from left to right: Is online political communication more than an echo chamber?." Psychological science 26, no. 10 (2015): 1531-1542.](http://journals.sagepub.com/doi/abs/10.1177/0956797615594620)

2015, Morales, A. J., Javier Borondo, Juan Carlos Losada, and Rosa M. Benito. ["Measuring political polarization: Twitter shows the two sides of Venezuela." Chaos: An Interdisciplinary Journal of Nonlinear Science 25, no. 3 (2015): 033114](https://arxiv.org/pdf/1505.04095.pdf)

    Important Contributions:
        A minority of influential users propogate their opinions
        Proposes an opinion probability density function
        Suggests a metric to quantify polarization
        Measure of polarization is inspired by electric dipole moment
        
    Dataset Used:
        Twitter data related to late Venezuelan President Hugo Chavez
        

    
    Analysis:
        Estimate opinions using the notion of elites and listeners
            Elites act like seeds
            Opnion of listeners depend on social interactions, and is the mean opinion value of neighbours
        A new measure of polarization named polarization index
        Network Analysis
            Used retweets to build a weighted and directed network
            Found elites using a small set of top 0.2% influential users who participated in most activities on the network
            Projected elite users on  a two dimensional space using word similarity
            Elites are assigned +1 or -1 polarity
            Opnions of rest (listeners) are based on social interaction simulation
            Finally evaluated polarization index 
            
            


2015, Williams, Hywel TP, James R. McMurray, Tim Kurz, and F. Hugo Lambert. ["Network analysis reveals open forums and echo chambers in social media discussions of climate change." Global Environmental Change 32 (2015): 126-138.](https://www.sciencedirect.com/science/article/pii/S0959378015000369)

2014, Akoglu, Leman. "Quantifying Political Polarity Based on Bipartite Opinion Networks." In ICWSM. 2014. http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.432.4647&rep=rep1&type=pdf

2013, Guerra, Pedro Henrique Calais, Wagner Meira Jr, Claire Cardie, and Robert Kleinberg. ["A Measure of Polarization on Social Media Networks Based on Community Boundaries." In ICWSM. 2013.(https://www.aaai.org/ocs/index.php/ICWSM/ICWSM13/paper/viewPDFInterstitial/6104Pedro/6360)

    Important Contributions:
        Systematic comparison of social-networks in polarized and non-polarized contexts.
        Modularity is not a good measure for learning antagonism between two groups as non-polarized gropus also contain modular communities
        Proposed a new polarization metric (by using information about nodes on community boundary)
        Found that polarized networks tend to have low concentration of hih-degree nodes at the boundary of communities
        

    
    Dataset Used:
        Twitter gun-control tweets
        University Friendshp Network
        Brazilian Soccer Supporters
        New York City Sports Teams
        Karate's Club
        2004 US Political Blogoshpere

    
    Analysis:
        Proposed a new polarization metric
        Tried the new metric on differnet dataset
        

2011, Conover, Michael, Jacob Ratkiewicz, Matthew R. Francisco, Bruno Gonçalves, Filippo Menczer, and Alessandro Flammini. ["Political polarization on twitter." ICWSM 133 (2011): 89-96](http://www.aaai.org/ocs/index.php/ICWSM/ICWSM11/paper/download/2847/3275)

    Important Contributions:
    Political retweets network exhibt segregated partisan netowork
    Mentions networks do not exhibit segregation, instead refelcts a single heterogeneous cluster. Mentions are used for bridging.
    Hashtags are used to reach politically opposed users
    
    Dataset Used:
    Twitter, containing tweets six weeks prior to 2010 US midterm elections (250,000 Tweets and 45,000 users)
    
    Analysis:
    Community Detection
        Created a list of politically relevant hashtags. Used these hashtags for filtering tweets.
        Built networks using retweets and mentions.
        Extracted the largest connected components from these neworks
        Used label propagation for community detection
        Seeded the algorithm with initial node labels for nodes exhibiting high eigen-vector modularity.
    Content Similarity
        For each user, built a vector that contains all hashtags used in his tweets, weighted by their frequency
        Found avarage similarity within clusters to be higher than across clusters
    Political Polarization
        Tried to identify left or right leaning
        Two authors annotated 1000 random users
        Used Cohen Kappa for annotation agreement
        Found that the majority of users express political identity
    Interaction Analysis
        To be added
        
        
    
    
    
2009, Gilbert, Eric, Tony Bergstrom, and Karrie Karahalios. ["Blogs are echo chambers: Blogs are echo chambers." In System Sciences, 2009. HICSS'09. 42nd Hawaii International Conference on, pp. 1-10. IEEE, 2009.](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.211.8065&rep=rep1&type=pdf)

# d) Tutorials
Awesome tutorial by Kiran  Garimella [Orignially shared on Dropbox](https://www.dropbox.com/s/labk5uu6e2j407h/Polarization%20on%20Social%20Media.pptx?dl=0#)


# e) Useful Websites
BuzzFeedNews [Partisan News Analysis](https://github.com/BuzzFeedNews/2017-08-partisan-sites-and-facebook-pages) 
BBC [The-myth-of-the-online-echo-chamber](http://www.bbc.com/future/story/20180416-the-myth-of-the-online-echo-chamber)

# f) Related Publications, but not necessarily on the topic above

# g) Citation of above papers in Bibtex (ToDo: This should be another file)
@article{garimella2018political,
  title={Political Discourse on Social Media: Echo Chambers, Gatekeepers, and the Price of Bipartisanship},
  author={Garimella, Kiran and Morales, Gianmarco De Francisci and Gionis, Aristides and Mathioudakis, Michael},
  journal={arXiv preprint arXiv:1801.01665},
  year={2018}
}


@article{Garimella:2018:QCS:3178568.3140565,
 author = {Garimella, Kiran and Morales, Gianmarco De Francisci and Gionis, Aristides and Mathioudakis, Michael},
 title = {Quantifying Controversy on Social Media},
 journal = {Trans. Soc. Comput.},
 issue_date = {February 2018},
 volume = {1},
 number = {1},
 month = jan,
 year = {2018},
 issn = {2469-7818},
 pages = {3:1--3:27},
 articleno = {3},
 numpages = {27},
 url = {http://doi.acm.org/10.1145/3140565},
 doi = {10.1145/3140565},
 acmid = {3140565},
 publisher = {ACM},
 address = {New York, NY, USA},
 keywords = {Controversy, echo chambers, filter bubble, polarization, twitter},
} 

@article{morales2015measuring,
  title={Measuring political polarization: Twitter shows the two sides of Venezuela},
  author={Morales, AJ and Borondo, Javier and Losada, Juan Carlos and Benito, Rosa M},
  journal={Chaos: An Interdisciplinary Journal of Nonlinear Science},
  volume={25},
  number={3},
  pages={033114},
  year={2015},
  publisher={AIP Publishing}
}

@inproceedings{guerra2013measure,
  title={A Measure of Polarization on Social Media Networks Based on Community Boundaries.},
  author={Guerra, Pedro Henrique Calais and Meira Jr, Wagner and Cardie, Claire and Kleinberg, Robert},
  booktitle={ICWSM},
  year={2013}
}

@article{conover2011political,
  title={Political polarization on twitter.},
  author={Conover, Michael and Ratkiewicz, Jacob and Francisco, Matthew R and Gon{\c{c}}alves, Bruno and Menczer, Filippo and Flammini, Alessandro},
  journal={ICWSM},
  volume={133},
  pages={89--96},
  year={2011}
}

@article{barbera2015tweeting,
  title={Tweeting from left to right: Is online political communication more than an echo chamber?},
  author={Barber{\'a}, Pablo and Jost, John T and Nagler, Jonathan and Tucker, Joshua A and Bonneau, Richard},
  journal={Psychological science},
  volume={26},
  number={10},
  pages={1531--1542},
  year={2015},
  publisher={Sage Publications Sage CA: Los Angeles, CA}
}


@article{WILLIAMS2015126,
title = "Network analysis reveals open forums and echo chambers in social media discussions of climate change",
journal = "Global Environmental Change",
volume = "32",
pages = "126 - 138",
year = "2015",
issn = "0959-3780",
doi = "https://doi.org/10.1016/j.gloenvcha.2015.03.006",
url = "http://www.sciencedirect.com/science/article/pii/S0959378015000369",
author = "Hywel T.P. Williams and James R. McMurray and Tim Kurz and F. Hugo Lambert",
keywords = "Social network analysis, Climate change, Polarisation, Echo chamber, Opinion leader"
}

@INPROCEEDINGS{Gilbert2009, 
author={E. Gilbert and T. Bergstrom and K. Karahalios}, 
booktitle={2009 42nd Hawaii International Conference on System Sciences}, 
title={Blogs are Echo Chambers: Blogs are Echo Chambers}, 
year={2009}, 
volume={}, 
number={}, 
pages={1-10}, 
keywords={Web sites;natural language processing;echo chambers;hand-coded blog comments;linguistic markers;natural language processing techniques;Blogs;Couplings;Humans;Lead;Milling machines;Natural language processing;Nominations and elections;Polarization;Psychology;Testing}, 
doi={10.1109/HICSS.2009.91}, 
ISSN={1530-1605}, 
month={Jan},}

@article{peterson2017echo,
  title={Echo Chambers and Partisan Polarization: Evidence from the 2016 Presidential Campaign},
  author={Peterson, Erik and Goel, Sharad and Iyengar, Shanto},
  year={2017}
}


@inproceedings{Gillani:2018:MME:3178876.3186130,
 author = {Gillani, Nabeel and Yuan, Ann and Saveski, Martin and Vosoughi, Soroush and Roy, Deb},
 title = {Me, My Echo Chamber, and I: Introspection on Social Media Polarization},
 booktitle = {Proceedings of the 2018 World Wide Web Conference},
 series = {WWW '18},
 year = {2018},
 isbn = {978-1-4503-5639-8},
 location = {Lyon, France},
 pages = {823--831},
 numpages = {9},
 url = {https://doi.org/10.1145/3178876.3186130},
 doi = {10.1145/3178876.3186130},
 acmid = {3186130},
 publisher = {International World Wide Web Conferences Steering Committee},
 address = {Republic and Canton of Geneva, Switzerland},
 keywords = {political polarization, randomized experiment, social networks},
} 

@article{takikawa2017political,
  title={Political Polarization in Social Media: Analysis of the" Twitter Political Field" in Japan},
  author={Takikawa, Hiroki and Nagayoshi, Kikuko},
  journal={arXiv preprint arXiv:1711.06752},
  year={2017}
}
@inproceedings{stewart2018examining,
  title={Examining trolls and polarization with a retweet network},
  author={Stewart, Leo G and Arif, Ahmer and Starbird, Kate},
  booktitle={Proc. ACM WSDM, Workshop on Misinformation and Misbehavior Mining on the Web (to appear). Accessed January},
  year={2018}
}
