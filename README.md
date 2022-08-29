# NFL Combine Model and Paper
## Project Overview
In this project, my good friend Jackson Filosa and I seek to understand the impact of NFL combine results on career performance.  We focus our study on quarterbacks and running backs.  We also produce a paper on our methodologies, findings, and conclusions.

For both quarterbacks and runningbacks, we look at the impact of five combine events: Forty Yard Dash, Vertical Jump, Broad Jump, Cone Drill, and Shuttle Run.  In asssessing quarterbacks, we use Quarterback Rating (QBR) as the response variable.  For runningbacks, we use Yards Per Carry (YPC).  For both positions, we also split the models into two groups: one only using first season metrics for the response varaible and another including a whole career average. 

The main takeaway from this analysis is that the combine (unsurprisingly) is not a good predictor of actual results.  When employing AIC-driven stepwise selection on the five above-mentioned predictor variables, statistically significant predictors exist for only runningbacks' career-wide YPC. The models predicting quarterbacks' first year and career-wide ratings, along with that of runningbacks' first year YPC all result in the empty model.

For runningbacks' carrer average YPC, the variables Forty Yard Dash and Broad Jump prove to be significant.  Interpreting the inclusion of the Forty Yard Dash is straight forward, as the explosive power tested for in the dash is greatly needed as a runningback.  However the significant Broad Jump relationship is negative in the regression, meaning that a longer jump corresponds with worse YPC performance.  This is, of course, somewhat harder to make sense of, and we deem it as likely spurious.  

For a more in depth analysis, please check out our [**full paper**](full_paper.pdf)!

## File Descriptions
[**NFL_Combine_Model.csv**](NFL_Combine_Model.csv): Code start to finish. Segmented into two streams: quarterback and runningback.  Both start with imports and data manipulation.  Then exploration and finally modelling. 

[**combine_data.csv**](combine_data.csv): Raw combine data from Kaggle.  This is then mathched with season performance data seperately for runningbacks and quarterbacks.

[**quarterback_data.csv**](quarterback_data.csv): Raw quarterback season data which is then matched via name to the combine data.

[**runningback_data.csv**](runningback_data.csv): Raw runningback season data which is then matched via name to the combine data.

[**full_paper.pdf**](full_paper.pdf): Associated paper which goes through the context, methodology, and results of the analysis.  
