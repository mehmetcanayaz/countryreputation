# Code and Data for Country Reputation and Corporate Activity  

I provide the necessary criteria for a 5% test on our IV procedure based on Lee, McCrary, Moreira, and Porter (2022).

The necessary content can be found in Section A.7 (see pages 13-20) of Lee, McCrary, Moreira, and Porter (2022)’s Online Appendix at http://www.princeton.edu/~davidlee/wp/tfNBERfinal_appendix.pdf. 


# GTD1_Main.dta: This file contains the terror dataset used in our analyses. As described in the Appendix, we download terror-related data from GTD. This dataset has 156,772 observations. We exclude attacks on military (targtype1==4), as they are endogenous. We also exclude unsuccessful attempts. We are left with 120,458 observations. We drop all attacks before 2000, because we want to have reasonable number of observations in the pre-treatment periods -particularly for events that occur in the beginning of 2000s. This is important, because we take the initial attacks between country pairs and our country image and news data is relatively unpopulated in the 1990s. We are left with 65,798 observations. We then identify initial attacks for each country pair. In so doing, we are left with 803 observations which are shared here.
