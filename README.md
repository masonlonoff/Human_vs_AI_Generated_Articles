# Human_vs_AI_Generated_Articles
A stylistic comparison of human and GPT 4o generated news articles

![image](https://miro.medium.com/v2/resize:fit:1400/1*T_uOLsOkuE5mxcUI7Lrtbg.png)


This repository contains the work done for my DS-GA 1015 - Text as Data final project at NYU. 

### Project Summary
This project investigates how GPT-4o writes about real-world news events that occurred after its training cutoff and how its writing style compares to professional human journalists. Using roughly 20 stylistic and linguistic features, I analyze differences in structure, readability, and language use across AI-generated and human-written articles.

I collected trusted news articles using the GDELT API and scraped full content using trafilatura. I then prompted GPT-4o to generate news articles using only the headlines from this human dataset. I extracted detailed features (e.g. POS ratios, entity mentions, readability scores, and lexical richness), built a Random Forest classifier to distinguish between sources, and applied SHAP values to interpret model behavior.

This project showcases skills in NLP, dataset generation, feature engineering, explainable ML, and stylistic content analysis which all offer insights into what makes AI writing feel different from human journalism, even when both describe the same real-world events.

#### File Breakdown

Below is a breakdown of each file you will find within the repository:
1) [Dataset Generation](https://github.com/masonlonoff/Human_vs_AI_Generated_Articles/blob/main/generating_articles.ipynb): This file contains the code for how I created both the human and GPT generated article datasets. It also includes the logic for how I filtered out unsuitable articles.
2) [Comparative Analysis](https://github.com/masonlonoff/Human_vs_AI_Generated_Articles/blob/main/comparative_analysis_of_articles.ipynb): This file contains the comparative analysis I did on the human and GPT generated articles. It also shows how I created the features that are later used in the Random Forest model.
3) [Random Forest classifier and SHAP values](https://github.com/masonlonoff/Human_vs_AI_Generated_Articles/blob/main/random_forest_and_shap_values.ipynb): This file contains the Random Forest classificstion model I used to determine article source. It also contains the SHAP values and feature importance scores to determine which features are most deterministic in determining if an article was writeen by humans or ChatGPT.
4) [Project Report](https://github.com/masonlonoff/Human_vs_AI_Generated_Articles/blob/main/Text%20as%20Data%20Final.pdf): This file contains the project report that was ultimately submitted.
