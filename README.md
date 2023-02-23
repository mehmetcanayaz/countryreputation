# Code and Data for Country Reputation and Corporate Activity  

Please find some of our hand-collected data and Stata/Python code below.

#### GTD1_Main.dta: 
This file contains the terror dataset used in our analyses. As described in the Appendix, we download terror-related data from GTD. This dataset has 156,772 observations. We exclude attacks on military (targtype1==4), as they are endogenous. We also exclude unsuccessful attempts. We are left with 120,458 observations. We drop all attacks before 2000, because we want to have reasonable number of observations in the pre-treatment periods -particularly for events that occur in the beginning of 2000s. This is important, because we take the initial attacks between country pairs and our country image and news data is relatively unpopulated in the 1990s. We are left with 65,798 observations. We then identify initial attacks for each country pair. In so doing, we are left with 803 observations which are shared here.



#### IPA1.dta:
We compile a list of promotion agencies using data from various resources. Part of our data comes from country promotion agencies from the website of World Association of Investment Promotion Agencies (WAIPA). WAIPA is an international organization established in 1995 to provide networking opportunities for agencies acting as a forum. It has 170 members from 130 countries. We identify agencies disclosed in the Members List section of the website, augmented with a set of promotion agencies listed in the Appendices of two UNCTAD papers (UNCTAD Advisory Paper 14, 1999 and UNCTAD Advisory Paper, 2001). The foundation years are obtained from individual agency websites, and in cases where this information is missing, we proxy it with promotion agency website creation years. 

#### tF value.ipynb:
The code estimates the critical value for our IV coefficient as in Lee, McCrary, Moreira, Porter (2022). We provide the necessary criteria for a 5% test on our IV procedure. The necessary content can be found in Section A.7 (see pages 13-20) of Lee, McCrary, Moreira, and Porter (2022)’s Online Appendix at http://www.princeton.edu/~davidlee/wp/tfNBERfinal_appendix.pdf. 

#### CountryNames.do:
This code cleans and revises (segment) country names based on other dataframes that are used in empirical analyses. It contains ~14,000 lines of code.
