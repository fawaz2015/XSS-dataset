# XSS dataset
Cross-site-scripting attacks: A Comprehensive dataset for AI techniques usage
![image](https://user-images.githubusercontent.com/13182456/163021488-345e295d-2e22-4331-bcc1-369f209f318f.png)

Abstract
Cross-site-scripting attacks are increasing dramatically nowadays, and there is no public and standard dataset intended to AI technologies used to combat such attacks. Building a new digital dataset of such attacks containing malicious and benign instances for training and testing AI models is worth attention. An extensive real-world data composed of 138,569 records have been constructed comprehensively and uniquely, including malicious and normal. Two phases have been taken to ensure standard raw data are representative and unbiased. First, the data were collected using a crawler employing a robust python scraping framework. The crawler applied a novel random walk and a random jumping method to crawl a sufficient variety of portions of the websites. The technique uses the probability of sample X, where X is crawled, and each observation's probabilities are inversely proportional to its PageRank. The top 50,000 websites ranking in Alexa feed the initial seed of the crawler. Then, by pre-configuration of the crawler, a maximum of 150,000 webpages are allowed to be crawled with 100 independent parallel walks and a jumping probability range between [0,1]. The second phase is to apply a uniform random sample method. The 100000 webpages are randomly selected among the total of 150000 webpages as uniform samples. The malicious webpages have been collected in a deterministic manner by designing a new crawler from two deference surcease, including XSSed and Open Bug Bounty. A total of 38,569 malicious samples are considered for this dataset. The initial 42 features were extracted by our dynamic-features extraction technique proposed in [2], While the comprehensive 167 features were extracted through enhanced dynamic features presented in [1]. Using the two stages of the Hybrid Feature Selection Approach (IG-SBS) proposed in [2], 66 features are obtained as an initial optimal subset. Two datasets are available; one is the complete data, including the and 167. It can be used all or part to train AI models. The other is a pre-processing dataset with 66 features that can also be used to train and test AI models through all or partial features or derive new features from the original dataset. Furthermore, the data set is large enough to train and test any model composed of 138,569 samples. 

--------------------------------------------------------------------------------
Cross-site-scripting attacks: A Comprehensive dataset for AI techniques usage

--------------------------------------------------------
References

If you used these datasets, please cite these related papers

1-Mokbal, F. M. M., Dan, W., Xiaoxi, W., Wenbin, Z., & Lihua, F. (2021). XGBXSS: An Extreme Gradient Boosting Detection Framework for Cross-Site Scripting Attacks Based on Hybrid Feature Selection Approach and Parameters Optimization. Journal of Information Security and Applications, 58, 102813.

2-Mokbal, F. M. M., Dan, W., Imran, A., Jiuchuan, L., Akhtar, F., & Xiaoxi, W. (2019). MLPXSS: an integrated XSS-based attack detection scheme in web applications using multilayer perceptron technique. IEEE Access, 7, 100567-100580.

