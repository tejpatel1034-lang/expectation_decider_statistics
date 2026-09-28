
# 📊 Expectation Decider – Mathematics & Advanced Statistics

> A practical probability and statistics project based on student academic data.

---

## 📌 Project Overview

**Expectation Decider** is a Mathematics and Advanced Statistics project that applies important concepts of **Probability and Statistics** to a real-world student dataset.

The project analyzes **200 students** using variables such as:

- Study Hours
- Attendance
- Group Discussion Participation
- Previous Test Score
- Final Exam Result

The main purpose of this project is to understand how probability and statistical concepts can be applied to real-world data and used to make meaningful observations.

---

## 🎯 Objectives

The main objectives of this project are:

1. Understand the basics of Probability.
2. Identify and explain different types of events.
3. Calculate Empirical and Theoretical Probability.
4. Define a Random Variable.
5. Construct a Probability Distribution.
6. Calculate Mean and Variance of a Random Variable.
7. Analyze events using a Venn Diagram.
8. Create and interpret a Contingency Table.
9. Calculate Joint, Marginal, and Conditional Probability.
10. Analyze relationships between events.
11. Understand Independent, Dependent, and Mutually Exclusive Events.
12. Apply Bayes Theorem to a real-world probability problem.
13. Use Python and Pandas for statistical analysis.

---

# 📂 Dataset

The project uses a dataset containing information about **200 students**.

### Dataset Features

| Column | Description |
|---|---|
| `Student_ID` | Unique identification number of each student |
| `study_hours` | Number of hours studied |
| `attendance` | Student attendance percentage |
| `group_discussion` | Whether the student participated in group discussion |
| `previous_test_score` | Score obtained in the previous test |
| `final_exam_pass` | Final exam result: Pass or Fail |

---

# 🛠️ Technologies Used

- 🐍 Python
- 📊 Pandas
- 🔢 NumPy
- 📓 Jupyter Notebook
- 📝 Markdown
- 📁 CSV Dataset
- 💻 Visual Studio Code

---

# 📚 Topics Covered

## 1. Probability Basics

### What is Probability?

Probability is a measure of how likely an event is to occur.

The value of probability lies between **0 and 1**.

### Formula

```text
Probability = Favorable Outcomes / Total Outcomes
````

### Example from the Dataset

There are:

* Total students = 200
* Students who passed = 7

Therefore:

```text
P(Pass) = 7 / 200
        = 0.035
        = 3.5%
```

So, the empirical probability of a student passing the final exam is **3.5%**.

---

# 2. Types of Events

An **event** is a specific outcome or collection of outcomes that we are interested in.

### Simple Event

An event containing a single outcome.

### Compound Event

An event containing two or more outcomes.

### Independent Event

Two events are independent when the occurrence of one event does not affect the probability of the other event.

### Dependent Event

Two events are dependent when one event can affect the probability of another event.

### Mutually Exclusive Events

Two events are mutually exclusive when they cannot occur at the same time.

For example:

```text
Pass and Fail
```

A student cannot be both Pass and Fail at the same time.

---

# 3. Empirical vs Theoretical Probability

## Empirical Probability

Empirical probability is calculated using actual observations or collected data.

### Example

From the dataset:

```text
Total Students = 200
Pass Students = 7
```

Therefore:

```text
P(Pass) = 7 / 200
        = 0.035
        = 3.5%
```

---

## Theoretical Probability

Theoretical probability is based on mathematical reasoning and possible outcomes.

### Example

For a fair six-sided die, the probability of getting 5 is:

```text
P(5) = 1 / 6
     ≈ 0.1667
     = 16.67%
```

### Difference

| Empirical Probability        | Theoretical Probability         |
| ---------------------------- | ------------------------------- |
| Based on actual observations | Based on mathematical reasoning |
| Uses collected data          | Uses possible outcomes          |
| Example: Student dataset     | Example: Rolling a die          |

---

# 4. Random Variable

A **Random Variable** is a variable whose value is determined by the outcome of a random experiment.

### Project Definition

For this project:

> Let X be the number of students who pass the final exam among 3 randomly selected students.

Therefore, possible values of X are:

```text
X = 0, 1, 2, 3
```

---

# 5. Probability Distribution

The probability of passing from the dataset is:

```text
p = 0.035
```

The probability of failing is:

```text
q = 1 - p
q = 1 - 0.035
q = 0.965
```

For 3 randomly selected students:

```text
n = 3
p = 0.035
q = 0.965
```

This follows a **Binomial Probability Distribution**.

### Binomial Formula

```text
P(X = x) = C(n,x) × p^x × q^(n-x)
```

### Probability Distribution

|  X | Probability |
| -: | ----------: |
|  0 |    0.898632 |
|  1 |    0.097779 |
|  2 |    0.003546 |
|  3 |    0.000043 |

---

# 6. Mean and Variance

For a Binomial Distribution:

### Mean

```text
E(X) = np
```

Therefore:

```text
E(X) = 3 × 0.035
     = 0.105
```

### Variance

```text
Variance = npq
```

Therefore:

```text
Variance = 3 × 0.035 × 0.965
         = 0.101325
```

### Results

```text
Mean     = 0.105
Variance = 0.101325
```

The mean represents the expected number of students passing among 3 randomly selected students.

---

# 7. Venn Diagram Analysis

Two events were analyzed using a Venn Diagram.

### Event A

```text
Study Hours > 10
```

### Event B

```text
Attendance > 80%
```

The dataset gives the following regions:

| Region          | Number of Students |
| --------------- | -----------------: |
| A Only          |                 40 |
| B Only          |                 46 |
| A ∩ B           |                 41 |
| Neither A nor B |                 73 |
| **Total**       |            **200** |

### Intersection

The intersection is:

```text
A ∩ B = 41
```

This means **41 students** studied for more than 10 hours and also had attendance above 80%.

---

# 8. Contingency Table

A contingency table is used to analyze the relationship between two categorical variables.

In this project, the variables are:

* Group Discussion
* Final Exam Result

### Contingency Table

| Group Discussion |    Fail |  Pass |   Total |
| ---------------- | ------: | ----: | ------: |
| No               |      57 |     0 |      57 |
| Yes              |     136 |     7 |     143 |
| **Total**        | **193** | **7** | **200** |

---

# 9. Joint Probability

Joint probability represents the probability of two events occurring together.

### Example

Probability of:

```text
Group Discussion = Yes
AND
Final Exam = Pass
```

There are 7 such students.

Therefore:

```text
P(Yes ∩ Pass) = 7 / 200
              = 0.035
              = 3.5%
```

---

# 10. Marginal Probability

Marginal probability represents the probability of a single event without considering another variable.

### Group Discussion = Yes

```text
P(Yes) = 143 / 200
       = 0.715
       = 71.5%
```

### Group Discussion = No

```text
P(No) = 57 / 200
      = 0.285
      = 28.5%
```

### Pass

```text
P(Pass) = 7 / 200
        = 0.035
        = 3.5%
```

### Fail

```text
P(Fail) = 193 / 200
        = 0.965
        = 96.5%
```

---

# 11. Conditional Probability

Conditional probability finds the probability of one event when another event is already known.

### Formula

```text
P(A|B) = P(A ∩ B) / P(B)
```

---

## Probability of Passing Given Group Discussion = Yes

```text
P(Pass | Yes) = 7 / 143
              ≈ 0.04895
              ≈ 4.90%
```

Therefore, among students who participated in group discussion, approximately **4.90% passed**.

---

## Probability of Passing Given Group Discussion = No

```text
P(Pass | No) = 0 / 57
             = 0%
```

Therefore, in this dataset, none of the students who did not participate in group discussion passed the final exam.

---

# 12. Relationship Analysis

The overall probability of passing is:

```text
P(Pass) = 3.5%
```

The conditional probability is:

```text
P(Pass | Group Discussion = Yes) = 4.90%
```

Since:

```text
4.90% ≠ 3.50%
```

the events do not satisfy the independence condition in this dataset.

Therefore, the dataset indicates that **Group Discussion and Final Exam Pass are not independent**.

### Mutually Exclusive?

No.

Group Discussion = Yes and Pass are not mutually exclusive because **7 students belong to both categories**.

---

# 13. Bayes Theorem

Bayes Theorem is used to update the probability of an event when new evidence or information becomes available.

### Formula

```text
P(A|B) = [P(B|A) × P(A)] / P(B)
```

---

## Given Values

The assignment provides:

```text
P(H | Pass) = 70%

P(H | Fail) = 40%

P(H) = 60%
```

We need to find:

```text
P(Pass | H)
```

---

## Step 1: Calculate P(Pass)

Using the Law of Total Probability:

```text
P(H) = P(H|Pass)P(Pass) + P(H|Fail)P(Fail)
```

Since:

```text
P(Fail) = 1 - P(Pass)
```

we get:

```text
0.60 = 0.70P(Pass) + 0.40(1 - P(Pass))
```

Solving:

```text
P(Pass) = 0.6667
```

Therefore:

```text
P(Pass) ≈ 66.67%
```

---

## Step 2: Apply Bayes Theorem

```text
P(Pass|H)
= [P(H|Pass) × P(Pass)] / P(H)
```

Substituting the values:

```text
P(Pass|H)
= (0.70 × 0.6667) / 0.60
```

Therefore:

```text
P(Pass|H) ≈ 0.7778
```

### Final Answer

```text
P(Pass|H) ≈ 77.78%
```

---

### Main Libraries

```python
import numpy as np
import pandas as pd
```

### Load Dataset

```python
df = pd.read_csv("students_data.csv")
```

### Check Dataset

```python
df.head()
```

### Dataset Shape

```python
df.shape
```

Expected shape:

```text
(200, 6)
```

---

# 📊 Key Project Results

| Analysis                         |       Result |
| -------------------------------- | -----------: |
| Total Students                   |          200 |
| Passed Students                  |            7 |
| Failed Students                  |          193 |
| Probability of Pass              |         3.5% |
| Attendance > 80%                 |  87 students |
| P(Attendance > 80%)              |        43.5% |
| Group Discussion = Yes           | 143 students |
| P(Group Discussion = Yes)        |        71.5% |
| Venn Intersection                |  41 students |
| Binomial Mean                    |        0.105 |
| Binomial Variance                |     0.101325 |
| P(Pass | Group Discussion = Yes) |        4.90% |
| P(Pass | Group Discussion = No)  |           0% |
| Bayes Result P(Pass | H)         |       77.78% |

---

# 🔍 Key Findings

From this project:

* The dataset contains **200 students**.
* **7 students passed** the final exam.
* The empirical probability of passing is **3.5%**.
* **87 students** had attendance greater than 80%.
* **143 students** participated in group discussion.
* **41 students** had both study hours greater than 10 and attendance greater than 80%.
* The expected number of passing students among 3 randomly selected students is **0.105**.
* Group Discussion and Final Exam Pass do not satisfy the independence condition in this dataset.
* The calculated Bayes Theorem result is approximately **77.78%**.

> **Note:** These findings describe this dataset only. They should not be interpreted as general conclusions about all students.

---

# 📁 Project Structure

```text
Expectation-Decider/
│
├── data/
│   └── students_data.csv
│
├── Expectation_Decider.ipynb
│
├── Rough_Work.pdf
│
├── README.md
│
└── Presentation/
    └── Project_Video
```

---

# 🎓 Learning Outcomes

After completing this project, I understood how to:

* Work with probability concepts.
* Calculate empirical probability.
* Understand theoretical probability.
* Define random variables.
* Construct probability distributions.
* Calculate expected value and variance.
* Apply binomial probability.
* Use Venn diagrams for event analysis.
* Create contingency tables.
* Calculate joint probability.
* Calculate marginal probability.
* Calculate conditional probability.
* Analyze event relationships.
* Apply Bayes Theorem.
* Use Python and Pandas for statistical analysis.
* Interpret statistical results from real-world data.

---

# 📝 Project Deliverables

This project contains:

* 📓 Jupyter Notebook
* 📊 Student Dataset CSV
* 📝 Rough Work PDF
* 📖 README Documentation
* 🎥 Project Presentation Video

---

# 👨‍💻 Author

**Tej Patel**

### Project

**Expectation Decider – Mathematics & Advanced Statistics**

```
