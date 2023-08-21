# Applying the Moneyball approach to Serie A Fantasy Football Data


This project aims to determine which features are deemed valuable by journalists to be a successful football player in Serie A.  

To accomplish this, we're using two data sources:
1. [FBref.com](https://fbref.com) – An online service collecting player-level objective stats.
2. [Fantacalcio.it](www.fantacalcio.it) – A [fantasy sport](https://en.wikipedia.org/wiki/Fantasy_sport) website measuring the players' performance in a subjective manner.

By combining these datasets, one can quantify which metrics affect the journalists' judgment when they assign their scores to players.  
To do so, an inference model is built to perform [regression analysis](https://en.wikipedia.org/wiki/Regression_analysis). The model measures each variable's impact on the output when the others are kept constant.  
In our case, the columns from data source (1) are used as independent variables `x`, while the scores in (2) represent the dependent variable `y`.

The results of this analysis can be helpful in many ways, including:
- Gauging the impact a new player (from a foreign league, the youth system, or lower tiers) could have in the Italian top tier.
- Learning where and how a player could improve their performance.
- Learning potential biases in how players are judged.
