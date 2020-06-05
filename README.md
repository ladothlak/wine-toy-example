# Wine Toy Example
Analyzing the red wine quality dataset from UCIML. This dataset is nice to practice on because it's all numerical (unless you consider the quality scores as being categorical--I've treated them as numerical) and has no missing values. In the attached notebook, I've min-max normalized all fields except quality and built a DNN regression model to the data. I haven't toyed too much with hyperparameters, as that is not the goal of this notebook.

Instead, the purpose is to offer feature contribution estimation with Shapley values. This is my first time using the open source shap library which you may find [here](https://github.com/slundberg/shap). As of 6/5/2020, I don't actually have any output for the shap values due to the compute-hungry nature of the process.

### What's Missing?
As I mentioned, I don't yet have shap value outputs. Because this is a compute-hungry process, I may need to make some concessions in its accuracy, such as kmeans clustering the data before feeding it into the DeepExplainer.

Additionally, due to the lack of shap value outputs, there are no beautiful graphs showing feature contribution. Once I have some shap values, though, this should be easy.
