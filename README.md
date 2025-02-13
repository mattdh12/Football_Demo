# Football_Demo

This notebook explores **fantasy football lineup optimization** with the goal of **maximizing the probability of reaching payout** in a contest. While fantasy football strategy is widely discussed in podcasts and media, this project takes a **data-driven approach** to analyze historical contest results and identify lineup characteristics correlated with success.

## Dataset  
The dataset consists of:  
- **Historical player projections** (e.g., projected points, projected ownership)  
- **Contest standings** (e.g., final scores, payout results)  

By examining how past lineups were constructed, the model evaluates features like **total projected points** and **total projected ownership** to estimate payout probability.

## Approach  
This problem was framed as a **classification task** (Made Payout vs. Missed Payout). Since a typical contest sees **~25% of lineups making payout and ~75% missing payout**, the dataset was **undersampled** to ensure that the model focuses on **identifying payout-viable lineups** rather than simply predicting majority-class outcomes.

## Key Findings  
The final model produced lineups with an **estimated 28% payout probability**—a slight improvement over the baseline 25%. However, this is a **proof of concept**, not an actionable contest strategy.  

While the model successfully increased payout probability, it **does not account for the top-heavy payout structure** of real contests, where maximizing expected return is more important than simply improving cash rates. **More effective strategies exist** for actual lineup construction.

This project is **for demonstration purposes only** and is not intended as an actionable strategy for real contests.
