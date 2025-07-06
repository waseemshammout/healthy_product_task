# healthy_product_task

Objective:
The goal is to build a classification model that focuses on identifying class +4 in the target column.
Note: The data is imbalanced, so the model must avoid overfitting to class -1, and instead aim for strong precision and recall on class +4, especially in the VALIDATE and TEST datasets.

📊 Data Info:
The column data_split separates the data into 3 sets: TRAIN, VALIDATE, and TEST.

✅ After Modeling & Filtering:
Once you've trained the model and filtered the samples predicted as +4 (or high-probability class +4), do the following:

For each data split (Train, Validate, Test), sum the remaining values in the target column after filtering.

Compare that sum with the total sum of target before feature selection and filtering in the same split.

The expectation is that in all 3 splits, the new sum should be positive and ideally higher or more stable than before selection.
