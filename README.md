# NFL Combine Model and Paper
## Project Overview
In this project, my good friend Jackson Filosa and I seek to understand how large of an impact NFL combine results have on career performance.  We focus our study on quarterbacks and running backs.  We also produced an article on our methodologies, findings, and conclusions.

For both quarterbacks and runningbacks, we look at the impact of five combine events: Forty Yard Dash, Vertical Jump, Broad Jump, Cone Drill, and Shuttle Run.  When asssessing quarterbacks, we used Quarterback Rating (QBR) as the response variable.  For runningbacks, we used Yards Per Carry (YPC).  For both positions, we also split the models into two groups: one with the response variable only from the player's first year of play and one including a career average. 

The main takeaway from this analysis is that the combine (unsurprisingly) is not a good predictor of actual results.  When employing AIC-driven stepwise selection on the five above-mentioned predictor variables, statistically significant predictors existed for only runningbacks' career-wide YPC, which quarterbacks' first year and career-wide rating, along with runningbacks' first year YPC all resulted in the empty model.

For runningbacks' carrer average YPC, the variables Forty Yard Dash and Broad Jump were significant in predicting Yards Per Carry across an RB's entire career results.  The interpretation of the Forty being included in the final model makes sense due to explosive power being needed as a runningback.  However the significant Broad Jump relationship is negative, meaning that a longer jump corresponds with worse YPC performance.  This is, of course, somewhat harder to interpret.  

## File Descriptions
[**raw_data.csv**](raw_data.csv): Raw data from Kaggle.  This is the only input file required to run the code.

[**journal_article.pdf**](journal_article.pdf): Associated article which goes through the context, methodology, and results of the analysis.  
