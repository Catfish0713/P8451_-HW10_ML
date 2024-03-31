# P8451_HW10_ML

In class, I summarized the Agier et al paper that used data from the HELIX harmonized birth cohorts in Europe. See Exercise10.docx for the summary. Previously, the research group working on HELIX launched a data challengeLinks to an external site. for exposomic data. They  invited researchers to share their analytic methods for high-dimensional data, including machine learning approaches. As part of that challenge, they released a dataset that represents their real HELIX data, similar to what was used in the Agier paper. The results from that challenge are published hereLinks to an external site.

An .Rdata file exposome.RData Download exposome.RDatahas been posted. It  contains 4 data.frames: exposome, phenotype, covariate and codebook. Exposome contains all of the environmental features measured on children. Phenotype contains health outcomes measured during the study. Covariate contains demographics and maternal information during pregnancy. Codebook is a detailed listing of all variables within the data frames. 

Your assignment this week is to begin to explore these data and develop a potential research question that could be feasibly addressed with them. An .RMD  Download .RMDhas been posted which includes sample code to load the .RData file and merge the data frames. (It also has code for examining interactions using a couple of different methods.) 

Please turn in a knit document that contains the following elements:

1. Examine the different features within the data frames and provide some descriptive measures (for continuous measures: means and ranges, for categorical/binary: frequency counts). Feel free to look at correlations between features, examine missingness, and other exploratory data analyses. You don't need to do this for all features within the data frames (although you could) but you should document summaries for at least 5 features from exposome and 1 feature from phenotype. These don't need to be formatted into tables or data frames. Just document that you've done some data exploration. 

2. Develop a single research question. It can be a prediction or hypothesis generating research question. It doesn't need to involve all features but it must involve at least one outcome from phenotype and 5 features from exposome (and covariates if relevant). This can be as simple or complex as a question as you want it to be. Clearly state the research question in a complete sentence outside of a code chunk, not as a comment within one.

3. Implement one algorithm from class that we've used previously to address your question. For this assignment, you should partition your data, develop the model in training (including hyperparameter turning and cross-validation) and then get final evaluation metrics in testing data. You can use package defaults for tuning or create your own vectors/grids. This is to keep getting practice with implementing algorithms so do as much as you would like and find useful.

4. Optional: Adapt the sample code for elastic net within the provided .RMD file to examine two-way interactions using the features and outcome you selected.