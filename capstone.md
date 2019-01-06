Evaluate Gradient Boosting Machines in modeling pipeline

### Exercise

The next model to be explored is Gradient Boosting Machines (GBM). GBM falls under decision tree models 
and like random forests can capture complex interactions in the dataset. GBM is a popular algorithm 
among Kagglers.

Using the sklearn package, GBM will be evaluated

### Instructions

- Import GBM from sklearn
- Create hyperparameter tuning step in the modeling pipeline
- Fit the model to the `X_train` and `y_train` and evaluate results

### Script

```python

from sklearn.feature_selection import ---------------
from sklearn.ensemble import ---------------
from sklearn import metrics
from sklearn import preprocessing
from imblearn.pipeline import ---------------


gbm = Pipeline([("imputer", preprocessing.Imputer(missing_values='NaN',
                                          strategy="mean",
                                          axis=1)),
                           ('variance', VarianceThreshold()),
                           ("scaler", preprocessing.StandardScaler()),
                           ('feature_selection',---------------,
                           ("model", ---------------)])
gbm.fit(-----,-----)

predicted = ------------
print "report: ", --------------

plot_importance(----,----)
plot_stretegy(---, X_valid, y_valid)

compare_models(------)
```
