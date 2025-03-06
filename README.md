# Xgboost

**What it does**
This is a repository where I have implemented Xgboost to derive a conclusion as whether th candidate can be approved for loan by looking at key parameters like age, income, years of employment, creddebt ratio and few other parameters.

**Things I learned**
Python coding
Correlation Heatmap & Pair Plot mapping
XgBoost

**High Level Inferences Made Based on Data**
1)There is not a strong corelation found between the education and income in this case. This contradicts the theoritcal rule, the more educated
you are the more income you earn, clearly that's not the case here.
2)There is significant corelation between credit debt, other debt and income, which makes perfect sense 
3) Another thing that is perplexing is not a strong corelation between debtinc % vs loan default, which makes me believe
most candidates with higher debtinc % have still managed to not being defaulted which then makes me to look at the PairPlot

Pair Plot Inference -  More than 80% defaulters belong to this bracket:
Candidates with ( Income < 100K && debtinc > 20% && employed for < 10yrs )
and so this is my most susceptible bucket which I will avoid in future.Any candidate that checks the above 3 criteria won't be approved for loan
