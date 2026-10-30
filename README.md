# Machine Intelligence notebooks, Autumn 2026

These are the notebooks for Lectures 7 to 9 of Machine Intelligence, the machine learning part of
the course. The course is CPH-SW5 at Aalborg University Copenhagen, Autumn 2026. The slides and
the lecture notes are on Moodle.

## How to open a notebook

- Click the *Open in Colab* button of a notebook. It opens in Google Colab, so you only need a
  Google account.
- Before you start, save your own copy with *File > Save a copy in Drive*. Colab opens the file
  from this repository, and the changes you make in that view are lost when you close it.
- The class notebooks read their data from this repository, so they need an internet connection
  when you run the first cells.
- To keep a copy on your computer, use *File > Download > Download .ipynb* in Colab.

## Lecture 7, Linear Regression I (Tuesday 27 October)

Go through these two notebooks before the lecture. They cover the Python and NumPy you need.

| Notebook | |
|---|---|
| Introduction to Python | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andresmasegosa/MI_E26/blob/main/lecture07/before-class/MI-L07-before-class-python.ipynb) |
| Introduction to NumPy | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andresmasegosa/MI_E26/blob/main/lecture07/before-class/MI-L07-before-class-numpy.ipynb) |

We do Exercises 1 to 4 in the lecture. Exercise 5 is homework before Lecture 8.

| Notebook | |
|---|---|
| Exercises 1 to 4, linear regression with one variable | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andresmasegosa/MI_E26/blob/main/lecture07/MI-L07-linear-regression.ipynb) |
| Exercise 5, vectorization with NumPy (at home, before Lecture 8) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andresmasegosa/MI_E26/blob/main/lecture07/MI-L07-vectorization.ipynb) |

The solutions are in `lecture07/solutions/`.

| Solution | |
|---|---|
| Solutions to Exercises 1 to 4 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andresmasegosa/MI_E26/blob/main/lecture07/solutions/MI-L07-linear-regression-SOLUTION.ipynb) |
| Solution to Exercise 5 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andresmasegosa/MI_E26/blob/main/lecture07/solutions/MI-L07-vectorization-SOLUTION.ipynb) |

## Lecture 8, Linear Regression II (Tuesday 3 November)

Do Exercise 5 of Lecture 7 before this lecture, if you have not done it yet. In the lecture we do
Exercises 2 and 4. Exercises 1, 3 and 5 are homework. Do Exercise 5 before the Kaggle notebook.

| Notebook | |
|---|---|
| Exercises 1 to 4, linear regression with multiple variables | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andresmasegosa/MI_E26/blob/main/lecture08/MI-L08-multiple-linear-regression.ipynb) |
| Exercise 5, vectorization with multiple variables (at home) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andresmasegosa/MI_E26/blob/main/lecture08/MI-L08-vectorization.ipynb) |

At the end of the lecture we start Kaggle competition 1. Open the Kaggle notebook and paste your
three functions from Exercise 5 into its Section 3. The invitation link to the competition is in
the Lecture 8 block on Moodle. The competition is not graded.

| Notebook | |
|---|---|
| Kaggle competition 1, bike rentals per hour | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andresmasegosa/MI_E26/blob/main/lecture08/MI-L08-kaggle.ipynb) |

The solutions to Exercises 2 and 4 will be posted on Moodle after the lecture. The solution to
Exercise 5 follows on Thursday 5 November, and those to Exercises 1 and 3 after Lecture 9.

## Lecture 9, Logistic Regression (Tuesday 10 November)

Its notebooks are added before the lecture.

## Credits

The class notebooks and the data file `houses.txt` adapt the labs of Andrew Ng's Machine
Learning Specialization (DeepLearning.AI and Stanford Online). The course functions of the Kaggle
notebook come from the same labs. The two before-class notebooks adapt the
[Scientific Python Lectures](https://github.com/jrjohansson/scientific-python-lectures) by
J.R. Johansson ([CC BY 3.0](https://creativecommons.org/licenses/by/3.0/)).

The data of Kaggle competition 1 is in `lecture08/data/Train.csv` and `lecture08/data/Test.csv`.
It comes from the [Bike Sharing dataset](https://archive.ics.uci.edu/dataset/275/bike+sharing+dataset)
by Hadi Fanaee-T, in the UCI Machine Learning Repository
([doi:10.24432/C5W894](https://doi.org/10.24432/C5W894)). The dataset is published under the
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) licence. Its authors ask users to cite
Fanaee-T and Gama (2013), "Event labeling combining ensemble detectors and background knowledge",
Progress in Artificial Intelligence
([doi:10.1007/s13748-013-0040-3](https://doi.org/10.1007/s13748-013-0040-3)).

We made both files from the dataset's `hour.csv`, with these changes:

- The columns `instant`, `casual` and `registered` are removed.
- `dteday` is renamed `date`, and `cnt` is renamed `count`.
- A new column `Id` gives each hour a random number.
- `Train.csv` has the hours of days 1 to 19 of each month. `Test.csv` has the other days, without
  `count`.
- The rows of each file are in random order.

The other columns are copied from `hour.csv` without changes.
