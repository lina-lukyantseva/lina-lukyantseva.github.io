---
permalink: /
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hello! I am co-founder and CTO at [Omnifold.ai](https://omnifold.ai). We're training multimodal prediction models for companies which make, distribute, and sell physical products. Our mission is to help businesses use all the data in their company and across the world to anticipate the future, so that they can eliminate waste and accelerate their growth.
<br>
<details>
  <summary><strong>We are hiring! ✨</strong></summary>
  <p>We are looking for a research engineer with strong ML theory/stats foundations + experience writing production code in python.</p>
  
  <p>What we do every day:</p>
  <ul>
    <li>find the right abstractions to model different industries and their supply chains</li>
    <li>work directly with customer data</li>
    <li>see our customers make real decisions based on Omnifold and learn from the real world feedback</li>
    <li>read papers and implement ideas, then come up with our own ideas for improvement -- because there is usually more relevant real world complexity than captured in academic setups</li>
    <li>collaborate with other researchers and engineers on the team, come up with a joint plan, then fully own and be responsible for your part of it</li>
  </ul>
  
  <p>We are onsite 5 days per week in SF. We are building fast and we are shipping fast 🚀 We are a team of people who <strong>LOVE</strong> finding elegant solutions to complex problems with measurable impact. If this resonates with you -- please reach out to learn more about the role!</p>
</details>
<br>
Previously I was a research engineer at Adept (acquired by Amazon) and a PhD student in economics & CS at Stanford.

<h1 id="Academic papers">Academic papers</h1>

<p><a name="bandits"><strong>Dynamic recommender systems via bandits with endogenous horizon</strong></a> [pdf coming soon]</p>
<details open>
  <summary><em>Abstract</em></summary>
  <div>In this paper I study the setting in which a digital platform (such as YouTube, Facebook or Duolingo) proposes content (such as videos, news feed or educational exercises) to its users sequentially. Each user has preferences over content categories (modeled as arms) that are initially unknown to the platform. The platform learns about these preferences dynamically, as it proposes more and more content. In contrast to the standard multi-arm bandits setting, the user Is not assumed to stay on the platform forever. Instead, after each period the user leaves the platform with some probability which depends on the quality of the received recommendations. This probability is allowed to be an arbitrary function of the arm history. The platform receives a reward every time a piece of content is consumed.
The platform's goal is to maximize the discounted sum of rewards obtained before the user leaves. I show that there exists an optimal index policy,determine the sequence of arms under the optimal policy, and design simulations to study the consequences of using misspesified models.</div>
</details>
<br>
<p><a name="logit"><strong>Good Unsystematic Mistakes</strong></a> [<a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4921967" target="_blank">pdf</a>]</p>
<details open>
  <summary><em>Abstract</em></summary>
  <div>We study the effects of consumers' unsystematic choice mistakes on market outcomes and consumer welfare. In the model, two firms produce goods of different quality and compete by choosing prices. Consumers observe the qualities and/or the prices with noise and make the unsystematic choice mistakes as a result. When the magnitude of mistakes grows, the lower-quality firm increases its price while the higher-quality firm initially reduces its price before increasing it. We show that this price reduction effect is almost always so strong that consumers eventually benefit from making a small amount of unsystematic mistakes despite sub-optimal choices and the increasing price of the lower-quality firm.</div>
</details>
<br>
<p><a name="data"><strong>Alternative data market regulation: navigating the fine line between finding alpha and insider trading</strong></a> [<a href="../files/Alternative_data_market_regulation.pdf" target="_blank">pdf</a>] [<a href="../files/data_market_slides.pdf" target="_blank">slides</a>]</p>
<details open>
  <summary><em>Abstract</em></summary>
  <div> While insider trading is strictly regulated, the regulation around trading on alternative data (such as credit/debit card transactions, app usage, geolocation, satellite imagery) remains vague. I study a model in which traders buy information from a monopolistic seller which is later used to trade in the financial market. My model is based on the single-period version of Kyle (1985). The data seller can sell the information of different quality, and the traders are heterogeneous in their ability to interpret the purchased signal. The regulator's utility function depends on the resulting price informativeness and the welfare of the liquidity traders. I show that trading on information bought through data markets has similar effects on price informativeness and the welfare of the liquidity traders as insider trading. Liquidity traders suffer even more if a small number of traders use the information than if only one trader uses it. I study optimal data seller's behavior in the absence of regulation and under different regulatory regimes. It is possible to ex ante increases both price informativeness and liquidity traders' welfare by (1)  requiring the data seller to sell the data through an auction with payments contingent on the traders' future profits and (2) setting a lower bound on the quantity that needs to be sold. </div>
</details>
<br>
<h1 id="Projects">Projects</h1>

<p><a name="position-bias"><strong>Position-bias-aware recommender systems</strong></a> [pdf available by request]</p>
Project @ LinkedIn
<details open>
  <summary><em>Abstract</em></summary>
  Training data for recommendation systems is biased: items shown at higher positions receive more interactions (such as clicks/applies in the context of job search on LinkedIn) than items shown at lower positions. Items shown at higher positions receive more interactions for two reasons. The first is because those items tend to be more relevant, and the second is because of position bias — people naturally pay more attention to items at the top. Training new iterations of recommendation systems on such data without properly accounting for position effects reinforces the existing biases in the model, resulting in worse recommendations.
  I propose a novel, model-based, approach to train recommender systems which accounts for position bias. My approach involves modifying the loss function to account for position effects explicitly without altering the data, and can be applied to any recommender system, including neural networks. Using a stylized recommender system, I demonstrate on LinkedIn data that my approach outperforms the method that modifies the training data, and outperforms commonly used model free approaches (even those which attempt to account for position bias).
</details>
