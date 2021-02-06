# MLApproaches
ML implementations in Multi-scale model for lignin biosynthesis in Populus Trichocarpa

In this work, I present the development of a Machine Learning algorithm that can be used as a part of the multi-scale model, developed by [Wang et al.](https://www.nature.com/articles/s41467-018-03863-z) and [Matthews](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1007197), designed to connect regulation across the different biological layers. As part of this model, the ML approach links the changes in the metabolic fluxes due to transgenic modifications of the monolignol transcript abundances with the 25 lignin and associated wood traits in the model tree *P. trichocarpa*. Through the study of lignin biosynthesis pathway, we aim to advance the strategic engineering of wood for timber, pulp, and biofuels.

In version 1 of the implementation, I have performed data preprocessing and trained each of the three chosen algorithms, XGB, SVR and kNN, in a pipeline and obtained optimal parameters for each model using GridSearchCV method. In addition to these steps, genetic algorithm has been added to the pipeline as a feature selection step in version 2, which significantly improved the performance of the models. After obtaining R^2 scores greater than the baseline scores of the original model by Mathews, I have implemented SHAP analysis on each of the three ML algorithms and analyzed the results for two of the phenotype traits: Lignin Content and Total Carbohydrate to Lignin (CL) ratio. Further detials of this work can be found in the [thesis dissertation](https://repository.lib.ncsu.edu/handle/1840.20/38374)
