# Ensemble Models

Ensemble models. Ensemble models are essentially models made up of other models. These component models are often models that are simpler than would be necessary to accurately predict the desired outcome on their own. In the case of Random Forest, those sub models are Decision Trees. Random Forest generates many Decision Trees and combines them to generate a single prediction via a voting process.

**Bagging** is one such ensemble technique. In bagging you take subsets of the data and train a model on each subset. Then the subsets are allowed to simultaneously vote on the outcome, either taking a majority or a mean. You just saw this in action with Random Forests, the most popular bagging technique.

Another ensemble technique is called **boosting**. Rather than build multiple models simultaneously like bagging, boosting uses the output of one model as an input into the next in a form of serial processing. These models then get daisy-chained together sequentially until some stopping condition is met. We’ll cover boosting methods later.

Lastly, **stacking** is a two phase process. In the first phase multiple models are trained in parallel. Then in the second phase those models are used as inputs into a final model to give your prediction. This approach combines the parallel approach embodied by bagging with the serial approach of boosting to create a hybrid of the two.

