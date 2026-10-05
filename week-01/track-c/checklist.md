# Track C — ML Fundamentals: Week 1 Checklist

**Track C** is for members who already know numpy, pandas, and matplotlib, and want to start
machine learning properly. This week covers the types of machine learning, data quality, train/test
splitting, the core learning tasks, and a first end-to-end scikit-learn fit/predict/evaluate loop.
Every day ends with a small hands-on deliverable. Flip each `- [ ]` to `- [x]` as you finish, then
commit your changes in your own fork.

**Scope:** the vocabulary, workflow, and tooling of supervised machine learning, from a clean
dataset to a judged model. By the end of the week you will have fit, predicted, and evaluated a real
scikit-learn model.

---

## Sunday 4 Oct 2026 — Setup + orientation

- [x] **Verify your stack** — confirm python, numpy, pandas, and matplotlib import and print versions. Why it matters: the ML ecosystem is version-sensitive, and you want to catch problems now.
  - https://numpy.org/doc/stable/user/quickstart.html
  - https://pandas.pydata.org/docs/getting_started/index.html
  - https://matplotlib.org/stable/tutorials/pyplot.html
- [x] **Set up a project folder with a clean structure** — `data/`, `src/`, `notebooks/`, `results/`, and a `requirements.txt`. Why it matters: reproducible ML starts with a reproducible folder.
  - https://pip.pypa.io/en/stable/
- [x] **Write your first scikit-learn environment** — `pip install scikit-learn`, then confirm the import and version. Why it matters: the model fitting you will do all week depends on a sane install.
  - https://scikit-learn.org/stable/getting_started.html
- [x] **Orientation: what machine learning is** — read an overview of the field, then write one paragraph defining supervised, unsupervised, and reinforcement learning in your own words. Why it matters: you cannot pick the right tool for a job until you know what the jobs are.
  - https://developers.google.com/machine-learning/crash-course
- [x] **Orientation: the ML workflow** — list the stages from data to deployment that this week will touch. Why it matters: it gives you a map before you start hiking.
  - **Deliverable:** a one-page note with the workflow stages and your field definitions.

## Monday 5 Oct 2026 — ML types and the workflow

- [x] **Supervised learning** — labeled data, prediction, and the two flavors: regression and classification. Why it matters: this week is almost entirely supervised.
  - https://developers.google.com/machine-learning/crash-course
  - https://scikit-learn.org/stable/modules/classification.html
- [x] **Unsupervised learning** — clustering and dimensionality reduction, and how it differs. Why it matters: not every problem has labels, and you will meet these methods soon.
  - https://developers.google.com/machine-learning/crash-course
- [x] **The machine learning workflow** — define the problem, get data, explore, clean, split, train, evaluate, tune, deploy, monitor. Why it matters: it is the same shape every week, and the discipline of it is what separates modeling from guesswork.
  - https://developers.google.com/machine-learning/crash-course
- [x] **Walk through the workflow on a dataset** — choose a small dataset, trace each stage on paper, and mark which you will do in detail next week. Why it matters: puts the terminology into practice immediately.
  - **Deliverable:** a printed workflow diagram with your dataset chosen.

## Tuesday 6 Oct 2026 — Data quality and leakage

- [ ] **Data quality dimensions** — completeness, consistency, accuracy, and timeliness. Why it matters: garbage in is the single biggest reason models fail in production.
  - https://scikit-learn.org/stable/common_pitfalls.html
- [ ] **Data leakage** — information that would not be available at prediction time, and why it inflates performance. Why it matters: leakage makes a model look brilliant in the lab and useless in the real world.
  - https://scikit-learn.org/stable/common_pitfalls.html
- [ ] **Detection and prevention** — train on a split version and a full version, and compare to show the gap. Why it matters: you will spot the telltale symptom during evaluation.
  - https://scikit-learn.org/stable/common_pitfalls.html
- [ ] **Clean a small dataset** — handle missing values, drop duplicated rows, and fix a type problem, then verify the shape before splitting. Why it matters: this is the exact first step you will run on every real project.
  - **Deliverable:** a cleaned dataset plus a short markdown summary of what you fixed and why.

## Wednesday 7 Oct 2026 — Train/test split

- [ ] **The purpose of a hold-out set** — why you evaluate on data the model never saw. Why it matters: this is the single most important idea in measuring real performance.
  - https://scikit-learn.org/stable/modules/cross_validation.html
- [ ] **Train/test split** — `train_test_split`, `test_size`, and `random_state`. Why it matters: reproducibility; you will call this today, and again in different shapes for the rest of the course.
  - https://scikit-learn.org/stable/modules/cross_validation.html
  - https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html
- [ ] **Stratified splits** — using `stratify` for classification so both halves keep the class balance. Why it matters: keeps your evaluation honest when classes are imbalanced.
  - https://scikit-learn.org/stable/modules/cross_validation.html
- [ ] **Compare split sizes** — train on 60/20/20 and on 80/20, and note how the estimates move. Why it matters: shows the tradeoff between data for learning and data for judging.
  - **Deliverable:** a short comparison table and a one-line conclusion.

## Thursday 8 Oct 2026 — Regression

- [ ] **What regression predicts** — a continuous number, and how it differs from classification. Why it matters: picking the right task family is step one.
  - https://scikit-learn.org/stable/modules/linear_model.html
- [ ] **Linear regression** — fit, coefficients, and interpretation on a small table. Why it matters: the baseline model you will understand deeply before moving to fancier ones.
  - https://scikit-learn.org/stable/modules/linear_model.html
  - https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html
- [ ] **Polynomial regression** — a few degrees higher, and why the fit can get dangerously good. Why it matters: introduces the bias-variance tension you will revisit in metrics.
  - https://scikit-learn.org/stable/modules/linear_model.html
- [ ] **Visualize the fit** — scatter plus the regression line, and a table of predictions vs actual. Why it matters: seeing a bad fit is worth a paragraph of reading.
  - **Deliverable:** a saved figure and a short diagnosis of the two models' errors.

## Friday 9 Oct 2026 — Classification

- [ ] **What classification predicts** — a category, and the probability vs label distinction. Why it matters: the metrics change completely between regression and classification.
  - https://scikit-learn.org/stable/modules/classification.html
- [ ] **Logistic regression** — decision boundary, probabilities, and the `predict_proba` method. Why it matters: it is the baseline classifier and the gateway to more advanced ones.
  - https://scikit-learn.org/stable/modules/linear_model.html
  - https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html
- [ ] **Decision trees** — how they split, and why they are a good second baseline. Why it matters: more interpretable and a natural contrast with linear models.
  - https://scikit-learn.org/stable/modules/tree.html
- [ ] **Compare a linear and a tree classifier** — on the same split, print accuracy and a confusion matrix for each. Why it matters: begins the habit of comparing models, not falling in love with one.
  - **Deliverable:** a short comparison report with a saved confusion matrix.

## Saturday 10 Oct 2026 — Metrics and bias-variance

- [ ] **Regression metrics** — MAE, MSE, and RMSE, and what each punishes. Why it matters: which number you optimize decides how your model treats error.
  - https://scikit-learn.org/stable/modules/model_evaluation.html
- [ ] **Classification metrics** — accuracy, precision, recall, F1, and ROC-AUC, plus when to prefer each. Why it matters: accuracy alone hides the failure mode you actually care about.
  - https://scikit-learn.org/stable/modules/model_evaluation.html
- [ ] **Bias and variance** — the two sources of error, and how they trade off. Why it matters: this is the mental model behind model selection and tuning.
  - https://scikit-learn.org/stable/auto_examples/model_selection/underfitting_overfitting.html
- [ ] **Diagnose a model** — pick one of your models from the week, describe its bias and variance in plain language, and state which you think is the bigger problem. Why it matters: turns the theory into a decision about what to do next.
  - **Deliverable:** a one-page diagnosis with the metric table that supports it.

## Sunday 11 Oct 2026 — Fit/predict/evaluate a first scikit-learn model

- [ ] **Run the full loop end to end** — define the data, split, choose a model, fit it, predict, and evaluate, with a real value at each step. Why it matters: it is the pattern you will repeat in every week of this program.
  - https://scikit-learn.org/stable/getting_started.html
- [ ] **Pick one model and justify it** — why you chose it for this problem, and what you would check next. Why it matters: model choice is a decision, not a default.
  - https://scikit-learn.org/stable/auto_examples/model_selection/underfitting_overfitting.html
- [ ] **Make a prediction on a new row** — feed a hand-written example through the fitted model and print the result. Why it matters: it proves the model does something it could not do before.
  - **Deliverable:** a runnable script plus its printed output for the new row.

## Monday 12 Oct 2026 — Review, catch-up, and worksheet

- [ ] **Review the week** — read back every day's deliverable and confirm each runs cleanly.
- [ ] **Catch up on anything missed** — re-read the scikit-learn user guide and the crash course if anything is unclear.
- [ ] **Complete the Track C worksheet** — fill in every row and the reflection section for week 1.
  - [Track C worksheet](week-01/track-c/worksheet.md)
