README – Dissertation Notebooks
Programme: University of London MSc Data Science
Submission: Supporting JupyterLab Notebooks (HTML exports)

This archive contains the HTML exports of all JupyterLab notebooks used to conduct
the experiments, data preparation, model training, synthetic data generation, and
evaluation described in the dissertation. Each notebook corresponds to a distinct
stage of the workflow and can be opened in any modern web browser.

Notebook Index
--------------

01_data_preparation.html
    - Loads raw dataset
    - Cleans and preprocesses features
    - Splits data into training and test pools
    - Performs initial exploratory checks

03_experimental_scenarios.html
    - xxx

03_ctgan_training_scenario_setup.html
    - Constructs the experimental grid (dataset sizes and imbalance ratios)
    - Creates un-augmented scenarios for CTGAN training
    - Prepares minority/majority subsets for each scenario

04_ctgan_hyperparameter_tuning.html
    - Trains CTGAN models across four representative scenarios
    - Evaluates candidate hyperparameter sets
    - Selects final configuration used in all experiments

05_ctgan_final_training.html
    - Trains CTGAN for each scenario in the experimental grid
    - Saves synthetic generators for augmentation

06_synthetic_generation.html
    - Generates synthetic minority samples for each augmentation level
    - Produces independent synthetic datasets per level
    - Stores outputs for downstream classifier training

07_synthetic_data_evaluation.html
    - Evaluates synthetic data quality (numerical and categorical)
    - Computes marginal statistics, correlation metrics, and mode-collapse checks
    - Summarises diagnostics for the final CTGAN configuration

08_classifier_training.html
    - Trains XGBoost classifiers for all scenarios and augmentation levels
    - Records performance metrics (Accuracy, F1, Recall, Precision, ROC AUC)

09_results_aggregation.html
    - Aggregates classifier results across the entire experimental grid
    - Produces tables and plots used in the dissertation
    - Computes deltas between augmented and un-augmented performance

10_final_experiments_and_plots.html
    - Generates final figures included in the dissertation
    - Performs additional checks (e.g., IR 243 behaviour)
    - Contains any supplementary experiments referenced in the Discussion

Notes
-----
- All notebooks are HTML exports and include full outputs, plots, and tables.
- No external dependencies are required to view the files.
- The notebooks are intended to support transparency and reproducibility of the
  experimental workflow described in the dissertation.

End of README
