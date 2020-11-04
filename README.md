# XIST

Correlation between X-Inactive Specific Transcript (XIST) and X chromosome genes in female and males across tissues.
Linear models performed in each tissue separately in males and females.

* Mean_LM.R fits linear models:
		* mean X expression ~ XIST counts
		* mean X-linked genes silenced in both Tukiainen et al. and Balaton et al. ~ XIST
		* mean X-linked silenced in Tukianen et al. ~ XIST
		* mean X-linked sielnced in Balaton et al. ~ XIST
		* mean X-linked silenced in at least one study ~ XIST
		* mean X-linked immune genes silenec in at least one study ~ XIST
		* mean X-linked variable escape genes in at least one study ~ XIST
		* mean X-linked variable escape genes in Tukianen et al. ~ XIST
		* mean X-linked variable escape genes in Balaton et al. ~ XIST
		* mean X-linked immune genes variable in at least one study ~ XIST
		* mean X-linked incompletely silenced (aka escape genes) in at least one study ~ XIST
		* mean X-linked incompletely silenced in Tukiainen et al. ~ XIST
		* mean X-linked incompletely silenced in Balaton et al. ~ XIST
		* mean X-linked immune genes incompletely silences in at least one study ~ XIST
		* mean All X-linked genes evaluated in Balaton et al. and Tukiainen et al ~ XIST
		* mean All X-linked genes not evaluated in either study ~ XIST
		* mean X-linked immune genes not evaulated in either study ~ XIST
		* mean PAR genes in Balaton et al. ~ XIST

* Mean_Plots.R plots the results from Mean_LM.R

* Median_LM.R does that same thing as Mean_LM.R, except it uses the median of the response variable.

* Median_Plots.R plots the results from Median_LM.R

* Sample_TPMs.R explores how many genes are left after applying various filtering thresholds.

* SummaryStats.R computes some summary statistics on the results of Mean_LM.R 
  
* The script in /Other_Genes include the following:
		* AR_Tissue.R does the same thing as Mean_LM.R, except the predictor variable is androgen receptor (AR)
		* AR_Plots.R makes the same plots as Mean_Plots.R, except with the results from AR_Tissue.R 
		* DDX3X_Tissue.R does the same thing as Mean_LM.R, except the predictor variable is DDX3X
		* DDX3X_Plots.R makes the same plots as Mean_Plots.R, except with the results from DDX3X_Tissue.R 
		* DDX3X_XIST.R fits a linear model: DDX3X ~ XIST in each tissue in males and females separately
		  and plots the results
		* Indiv_LM.R can be ignored. We realized fitting LMs by tissue makes more sense than by individual.
