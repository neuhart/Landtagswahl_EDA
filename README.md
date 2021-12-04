# Landtagswahl_EDA
Done in Jupyter
Exploratory data analysis of the state election results of  Upper Austria in Linz 
Data from LT21Sprengel.csv 
Contains results of the 2021 state election in Upper Austria (Oberösterreich) constrained to the votes of Upper Austria's capital city Linz

What I did:
Starting off the exploratory data analysis, I took a look at the data structure (e.g. names of columns, which columns are qualitative/quantitative, etc.). I also looked into some statistical metrics such as the mean, std, etc. of each column to get a better unterstanding of the distribution of the numerical data.
After some preprocessing of the data such as getting rid of parties with less than 5% of the total vote, I plotted the election results. 
To find out if there are any significant correlations between votes and population size of a 'Wahlsprengel' for any party, I created regression plots for each party.
Additionally, I drew the correlation matrix of the number of people elligible to vote and all five partys. 
To gain potential further insight, I plotted the number of 'Wahlsprengel' won per party.

Findings:
-Regression plots:
The Austrian people's party (ÖVP) shows a relatively large negative correlation in Linz. This is not very surprising since this party usually also performs better in less densely populated (rural) areas. 
But what is more surprising is that the election success per 'Wahlsprengel' of the Austrian social democratic party (SPÖ) tends to negatively correlate with population size. But this observation could be misleading considering the high leverage points of 'Wahlsprengel' with low population size where the social democrats performed very well.
-Correlation Matrix:
GRÜNE and NEOS show high positive correlations. Both are high negative correlated to SPÖ and FPÖ. ÖVP also seems to be negatively correlated to SPÖ and FPÖ but shows almost no correlation with GRÜNE and NEOS. 
-Wahlsprengel results: 
Even though ÖVP won the election in Linz, SPÖ won more Wahlsprengel in total. This can at least in part be explained by the high negative correlation of ÖVP's votes and population size per Wahlsprengel. 
