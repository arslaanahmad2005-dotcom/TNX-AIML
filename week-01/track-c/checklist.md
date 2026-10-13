# Track C — ML Fundamentals: Week 1 Checklist

**Track C** is for members who already have some Python and want to start machine learning properly.
This week first **brushes up the three core libraries — numpy, pandas, matplotlib — one library per
day**, each with the video's own dataset and capstone worksheet, and then covers **ML fundamentals**:
what ML is, the types of ML, EDA, data cleaning, preprocessing, and feature engineering/selection.
Every day ends with a hands-on deliverable. Flip each `- [ ]` to `- [x]` as you finish, then commit
your changes in your own fork.

**Week:** Mon 12 Oct 2026 → Mon 19 Oct 2026 · **7 topic days** (Mon–Sun) + a review Monday.
**Days 1–3 — library brush-up (one library a day):**

- numpy — [video](https://youtu.be/Utgwk0r9Zq4) · [repo](https://github.com/AkarshVyas/Numpy-Youtube)
- pandas — [video](https://youtu.be/QUaSmqBeR9w) · [repo](https://github.com/AkarshVyas/Pandas-Youtube)
- matplotlib & seaborn — [video](https://youtu.be/-jTD74eEy2I) · [repo](https://github.com/AkarshVyas/Data-Visualization-Youtube)

**Days 4–7 — ML fundamentals:** [Complete Machine Learning Course playlist](https://www.youtube.com/playlist?list=PLaldQ9PzZd9qT0KsKJ7yCq70iFFP3MFJ5),
starting with [Part 1 — Foundation](https://youtu.be/1L420xXpDTg).

> Each day's questions live in the matching file under [`worksheet/`](worksheet/README.md), e.g. Day 1
> questions are in [`worksheet/day-1.md`](worksheet/day-1.md).

---

## Day 1 — Monday 12 Oct 2026 — numpy

**Watch:** [numpy — Complete Data Science Course (2 h)](https://youtu.be/Utgwk0r9Zq4)
**Dataset & capstone:** the video description links [AkarshVyas/Numpy-Youtube](https://github.com/AkarshVyas/Numpy-Youtube),
which contains `Arrays.ipynb`, `array_indexing.ipynb`, `array_operations.ipynb`, and the **`exersises.ipynb` worksheet**.

- [x] **Notebooks (setup)** — `0:28` · get Jupyter/Colab running. Why it matters: every day this week runs in a notebook.
- [x] **NumPy arrays** — `19:28` · creating arrays, `shape`, `dtype`, `arange`/`linspace`. Why it matters: the whole data stack rests on arrays.
- [x] **Indexing & slicing** — `46:57` · selecting rows, columns, and blocks of an array. Why it matters: reading data starts with selecting it.
- [x] **Array operations & broadcasting** — `1:04:12` · element-wise maths and how numpy aligns shapes. Why it matters: the core pattern behind nearly every numeric operation.
- [x] **Complete the `exersises.ipynb` worksheet** — `1:30:01` · the exercise set at the end of the video. Why it matters: it is the day's hands-on test.
- **Deliverable:** your completed `exersises.ipynb` plus the Day 1 answers in [`worksheet/day-1.md`](worksheet/day-1.md).

## Day 2 — Tuesday 13 Oct 2026 — pandas

**Watch:** [pandas — Complete Data Science Course (2 h 23 m)](https://youtu.be/QUaSmqBeR9w)
**Dataset & capstone:** the description links [AkarshVyas/Pandas-Youtube](https://github.com/AkarshVyas/Pandas-Youtube)
(see `2)DataFrames.ipynb`, `3)MissingData.ipynb`, `5)GroupByAggregation.ipynb`), and the video ends with a **Data Capstone Project**.

- [x] **Series & DataFrames** — `3:32` and `11:27` · the two pandas containers and loading a CSV. Why it matters: pandas is the standard way to work with tables.
- [x] **Missing data** — `35:20` · detecting, dropping, and filling missing values. Why it matters: real datasets are incomplete.
- [x] **Merging, joining & concatenation** — `45:33` and **group-by / pivot tables** — `57:46` and `1:08:02`. Why it matters: combining and summarising tables is most of data work.
- [x] **Feature extraction project** — `1:27:58` · build the project from the video.
- [x] **Data capstone project** — `1:56:19` · the end-of-video worksheet. Why it matters: it is the day's hands-on test.
- **Deliverable:** your completed capstone notebook plus the Day 2 answers in [`worksheet/day-2.md`](worksheet/day-2.md).

## Day 3 — Wednesday 14 Oct 2026 — matplotlib & seaborn

**Watch:** [Data Visualization — Matplotlib & Seaborn (2 h 35 m)](https://youtu.be/-jTD74eEy2I)
**Dataset & capstone:** the description links [AkarshVyas/Data-Visualization-Youtube](https://github.com/AkarshVyas/Data-Visualization-Youtube),
which contains `IPL.csv`, the plot notebooks, and the **`IPL_Capstone_Project.ipynb`** worksheet.

- [ ] **Matplotlib basics** — `5:29` · line, bar, and scatter plots with labels and titles. Why it matters: a picture is the fastest way to check your data.
- [ ] **Distribution, categorical & matrix plots** — `41:21`, `1:05:57`, `1:23:36`, and **regression plots** — `1:37:09`. Why it matters: each chart type answers a different question.
- [ ] **Plotly & Cufflinks (interactive)** — `1:45:09` · a quick look at interactive plots.
- [ ] **Complete the IPL capstone project** — `1:55:53` · the end-of-video worksheet on `IPL.csv`. Why it matters: it is the day's hands-on test.
- **Deliverable:** your completed `IPL_Capstone_Project.ipynb` plus the Day 3 answers in [`worksheet/day-3.md`](worksheet/day-3.md).

## Day 4 — Thursday 15 Oct 2026 — What ML is, and the types of ML

**Watch:** ML Part 1 — Foundation · [2:54 – 25:20](https://youtu.be/1L420xXpDTg?t=174)

- [ ] **What machine learning is** — `2:54` · learning patterns from data instead of writing rules.
- [ ] **Real-life applications & traditional programming vs ML** — `6:52` and `8:47`. Why it matters: it frames when ML is the right tool at all.
- [ ] **AI vs ML vs DL** — `10:22` · where each fits.
- [ ] **Types of machine learning** — `14:34` · supervised, unsupervised, reinforcement. Why it matters: you cannot pick a tool until you know the job.
- **Deliverable:** a one-paragraph summary of supervised vs unsupervised vs reinforcement, with one example of each, plus Day 4 answers in [`worksheet/day-4.md`](worksheet/day-4.md).

## Day 5 — Friday 16 Oct 2026 — The ML steps, EDA, and data cleaning

**Watch:** [25:20 – 42:30](https://youtu.be/1L420xXpDTg?t=1520)

- [ ] **Steps for making an ML model** — `25:20` · the end-to-end workflow. Why it matters: it is the same shape for every project.
- [ ] **EDA (exploratory data analysis)** — `28:15` · shapes, types, distributions, and correlations. Why it matters: you must look before you model.
- [ ] **Data cleaning** — `33:45` · missing values, duplicates, and wrong types. Why it matters: garbage in is the biggest reason models fail.
- **Deliverable:** run EDA and cleaning on a small CSV of your choice (shape, `info()`, missing-value counts, duplicates removed) and write a short summary, plus Day 5 answers in [`worksheet/day-5.md`](worksheet/day-5.md).

## Day 6 — Saturday 17 Oct 2026 — Preprocessing, feature engineering & selection

**Watch:** [42:30 – 1:01:42](https://youtu.be/1L420xXpDTg?t=2550)

- [ ] **Data preprocessing** — `42:30` · encoding categories and scaling numbers. Why it matters: models only understand numbers.
- [ ] **Feature engineering** — `54:10` · creating new, more useful columns. Why it matters: better features often beat better models.
- [ ] **Feature selection** — `57:58` · dropping what does not help. Why it matters: fewer, better columns reduce noise and overfitting.
- **Deliverable:** take your cleaned CSV from Day 5, encode its categorical columns, scale a numeric column, and drop one weak feature — with a one-line reason for each step, plus Day 6 answers in [`worksheet/day-6.md`](worksheet/day-6.md).

## Day 7 — Sunday 18 Oct 2026 — Foundation projects 1 & 2

**Watch:** [1:01:42 – 2:42:43](https://youtu.be/1L420xXpDTg?t=3702)

- [ ] **Project 1** — `1:01:42` · follow the full foundation project end to end.
- [ ] **Project 2** — `2:07:15` · the second project across the whole workflow.
- [ ] **Rebuild one project on your own dataset** — reuse the same steps on a different CSV so the workflow sticks.
- **Deliverable:** both project notebooks plus the Day 7 answers in [`worksheet/day-7.md`](worksheet/day-7.md).

## Monday 19 Oct 2026 — Review, catch-up, and worksheet completion

- [ ] **Review the week** — read back every day's deliverable and confirm each one runs.
- [ ] **Catch up on anything missed**, using the official library docs and the ML crash course as references.
- [ ] **Complete every day worksheet** you have not finished yet.
- [ ] **Fill the week reflection** at the end of the checklist.

---

## Documentation (read after all 7 days)

Work through these once you have finished the days above — they are the official references you will
keep coming back to.

- **NumPy quickstart:** https://numpy.org/doc/stable/user/quickstart.html
- **NumPy absolute beginners:** https://numpy.org/doc/stable/user/absolute_beginners.html
- **pandas getting started:** https://pandas.pydata.org/docs/getting_started/index.html
- **pandas 10 minutes to pandas:** https://pandas.pydata.org/docs/user_guide/10min.html
- **Matplotlib pyplot tutorial:** https://matplotlib.org/stable/tutorials/pyplot.html
- **Seaborn tutorial:** https://seaborn.pydata.org/tutorial.html
- **Google ML crash course:** https://developers.google.com/machine-learning/crash-course
- **scikit-learn — getting started:** https://scikit-learn.org/stable/getting_started.html
- **scikit-learn — common pitfalls (data leakage):** https://scikit-learn.org/stable/common_pitfalls.html

## Week reflection

- **Biggest takeaway this week:** _______________________________________________
- **Blocker or stumbling point:** _______________________________________________
- **Open question:** _______________________________________________
- **One topic I want to revisit:** _______________________________________________
- **Goal for next week:** _______________________________________________
