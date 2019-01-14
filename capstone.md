Evaluate Gradient Boosting Machines in modeling pipeline

### Exercise

The next model to be explored is Gradient Boosting Machines (GBM). GBM falls under decision tree models
and like random forests can capture complex interactions in the dataset. GBM is a popular algorithm among Kagglers.

### Instructions

- Create a modeling pipeline that uses GBM algorithm in the modeling step and has a hyperparameter tuning step
- Fit the model to the `X_train` and `y_train` and evaluate results on `X_valid` and `y_valid`

### Script

```python
from sklearn.ensemble import GradientBoostingClassifier
from sklearn.model_selection import GridSearchCV

# Create the model
algorithm = Pipeline([('feature_selection',---------------,
                ("model", ---------------)])
param_grid = {'max_depth':range(5,16,2),'min_samples_split':range(200,1001,200)}
gbm = GridSearchCV(-----------, param_grid=------------,cv=5)

# Fit model and evaluate results
gbm.fit(-----,-----)
print "report: ", --------------
plot_importance(----,----)
```
