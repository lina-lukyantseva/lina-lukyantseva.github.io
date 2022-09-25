---
permalink: /
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hello! I am a 5th year PhD student at Stanford University, advised by  [Andrzej Skrzypacz](https://www.gsb.stanford.edu/faculty-research/faculty/andrzej-skrzypacz). 
My research focus is on the intersection of economics and computer science – specifically, I am interested in how to combine the 
structure of microeconomic models with the flexibility of ML algorithms to develop AI systems which are general, 
interpretable, and incentive aligned. 

Most recently, I was an intern at LinkedIn, on the Economics / AI team. LinkedIn uses recommender systems across its platform - 
for example, to offer jobs to candidates. One of the challenges of recommender systems is position bias – listings which are displayed 
in a more favorable position are more likely to be selected, even if they are less relevant. I developed a [novel approach](#position-bias) to correcting 
for position bias, by combining economic techniques for parameter estimation with ML-based methods for training.

Prior to Linkedin, I was working on [“Recommender systems via bandits with endogenous horizon”](#bandits), a topic in Multi-Armed Bandits. 
A common problem faced by content platforms is that consumers can completely exit the platform if they are not satisfied with the content 
they see – traditional bandit algorithms do not account for this. I developed a theoretical approach to model this scenario by expanding 
on the Gittins Index, and implemented simulations to demonstrate under which conditions it is particularly important to account for the time 
horizon endogeneity. 

Before that, I worked on papers in mechanism design and decision theory, including [regulating markets for data](#data) and [modeling consumers
whose behavior is not fully rational](#logit).

If you’d like to connect, please reach out to me at lina.lukyantseva ‘at’ gmail 'dot' com.

<h1 id="Working papers">Working papers</h1>

<p><a name="bandits"><strong>Dynamic recommender systems via bandits with endogenous horizon</strong></a> [pdf coming soon]</p>
<details open>
  <summary><em>Abstract</em></summary>
  <kbd>In this paper I study the setting in which a digital platform (such as YouTube, Facebook or Duolingo) proposes content (such as videos, news feed or educational exercises) to its users sequentially. Each user has preferences over content categories (modeled as arms) that are initially unknown to the platform. The platform learns about these preferences dynamically, as it proposes more and more content. In contrast to the standard multi-arm bandits setting, the user Is not assumed to stay on the platform forever. Instead, after each period the user leaves the platform with some probability which depends on the quality of the received recommendations. This probability is allowed to be an arbitrary function of the arm history. The platform receives a reward every time a piece of content is consumed.
The platform’s goal is to maximize the discounted sum of rewards obtained before the user leaves. I show that there exists an optimal index policy,determine the sequence of arms under the optimal policy, and design simulations to study the consequences of using misspesified models.</kbd>
</details>
<br>
<p><a name="logit"><strong>Unexpected effects of consumer sophistication on competition and welfare in asymmetric Bertrand olygopolies</strong></a> [pdf coming soon]</p>
<details open>
  <summary><em>Abstract</em></summary>
  <kbd>This paper studies a market in which two firms produce the same good but can have different quality. Consumers observe the quality imperfectly —  the perceived quality is equal to the true quality plus some error. The firms set prices, and then each consumer buys the good from the firm which gives her a higher perceived consumer surplus. The resulting demand takes logit form. The variance of the error term is interpreted as the degree of consumer sophistication — when the variance is low, the perceived quality is close to the true quality, and when the variance is high, the perceived quality can be very far from the true quality since it is mostly determined by a random draw of the error term. I show that when firms are symmetric (i.e. have the same quality) expected consumer surplus is increasing in consumer sophistication. However, when firms are asymmetric, consumers benefit from being slightly unsophisticated, which is a surprising result. This happens because the firm with a higher quality needs to set a lower price in order to make it more obvious to the consumers that they are the better firm. 
I also analyze an alternative interpretation of the same mathematical model in which the random component of the perceived quality is not an observation error but rather a part of consumer’s utility (a.k.a. random utility model). </kbd>
</details>
<br>
<p><a name="data"><strong>Alternative data market regulation: navigating the fine line between finding alpha and insider trading</strong></a> [<a href="../files/Alternative_data_market_regulation.pdf" target="_blank">pdf</a>] [<a href="../files/data_market_slides.pdf" target="_blank">slides</a>]</p>
<details open>
  <summary><em>Abstract</em></summary>
  <kbd> While insider trading is strictly regulated, the regulation around trading on alternative data (such as credit/debit card transactions, app usage, geolocation, satellite imagery) remains vague. I study a model in which traders buy information from a monopolistic seller which is later used to trade in the financial market. My model is based on the single-period version of Kyle (1985). The data seller can sell the information of different quality, and the traders are heterogeneous in their ability to interpret the purchased signal. The regulator’s utility function depends on the resulting price informativeness and the welfare of the liquidity traders. I show that trading on information bought through data markets has similar effects on price informativeness and the welfare of the liquidity traders as insider trading. Liquidity traders suffer even more if a small number of traders use the information than if only one trader uses it. I study optimal data seller's behavior in the absence of regulation and under different regulatory regimes. It is possible to ex ante increases both price informativeness and liquidity traders’ welfare by (1)  requiring the data seller to sell the data through an auction with payments contingent on the traders’ future profits and (2) setting a lower bound on the quantity that needs to be sold. </kbd>
</details>
<br>
<h1 id="Projects">Projects</h1>

<p><a name="position-bias"><strong>Position-bias-aware recommender systems</strong></a> [pdf coming soon]</p>
intern project @ LinkedIn
<details open>
  <summary><em>Abstract</em></summary>
  <kbd>Training data for recommendation systems is biased: items shown at higher positions receive more interactions (such as clicks/applies in the context of job search on LinkedIn) than items shown at lower positions. Items shown at higher positions receive more interactions for two reasons. The first is because those items tend to be more relevant, and the second is because of position bias — people naturally pay more attention to items at the top. Training new iterations of recommendation systems on such data without properly accounting for position effects reinforces the existing biases in the model, resulting in worse recommendations.
  I propose a novel, model-based, approach to train recommender systems which accounts for position bias. My approach involves modifying the loss function to account for position effects explicitly without altering the data, and can be applied to any recommender system, including neural networks. Using a stylized recommender system, I demonstrate on LinkedIn data that my approach outperforms the method that modifies the training data, and outperforms commonly used model free approaches (even those which attempt to account for position bias).</kbd>
</details>
