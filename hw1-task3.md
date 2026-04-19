# Homework 1 Task 3

---

Answer the following questions based on exercises from *An Introduction to Statistical Learning with Applications in Python*.

## Chapter 2.4 Exercises

---

### Exercise 1 (ISLP exercise 2)

Explain whether each scenario is a **classification or regression** problem, and indicate whether we are most interested in **inference or prediction**. Finally, provide **n** (size of observation dataset) and **p** (number of predictors).

**(a)**  We collect data on 200 protected marine reserves worldwide. For each reserve we record species richness, reserve size, years since establishment, enforcement budget, and proximity to human settlements. We are interested in understanding which factors affect species richness.

> **Your Answer:**
Scenario `a` is a *regression* problem in which we care about *inferring* which factors affect species richness. There are 200 (n) sample marine reserves and we have 4 predictors (p)

---

**(b)** A conservation agency wants to know whether a proposed habitat corridor will successfully support wildlife movement or fail to do so. They collect data on 30 previously established corridors. For each corridor they have recorded whether wildlife movement was successful or unsuccessful, corridor width, length, surrounding land use type, and eight other variables.

> **Your Answer:**
Scenario `b` is a *classification* scenario (binned 0-1 successful/unsuccessful) in which we care about whether corridor success can be *predicted* by 11 predictors (p). We accomplish this by collecting data on 30 (n) corridors. 

---

**(c)** We are interested in predicting weekly average ground-level ozone concentration in a coastal city. We collect weekly data for all of 2019. For each week we record average ozone concentration, sea surface temperature, wind speed, solar radiation, and atmospheric

> **Your Answer:**
Scenario `c` is an *regression* scenario in which we care about *predicting* ozone concentration. To accomplish this we collect weekly data for all of 2019 (52 weeks = n) of 4 predictors (p)

---

### Exercise 2 (ISLP exercise 5)

What are the advantages and disadvantages of a very flexible (versus a a less flexible) approach for regression? Under what circumstances might a more flexible approach be preferred to a less flexible approach? When might a less flexible approach be preferred?

> **Your Answer:**
A specific model will adapt to your data, and give you more accurate results to your current data. This may make better predictions, but it may not scale as you add data. A more flexible model can handle scaling (better for inference), but may not account for as much variation in your points. Flexible models risk overfitting, inflexible models risk underfitting. 
---

### Exercise 3 (ISLP exercise 6)

Describe the differences between a **parametric** and a **non-parametric** statistical learning approach. What are the **advantages** of a parametric approach to regression or classification (as opposed to a non-parametric approach)? What are its **disadvantages**?

> **Your Answer:**
Parametric models have a specific shape (eg: normal), and estimate a *fixed* set of parameters. The advantages of parametric models are that they need less data and are easily interpretable, while the disadvantages are that if the assumptions are violated the model can collapse. Non-parametric models do not assume a shape nor do they have fixed parameters, making them more flexible. The advantages of non-parametric models are that they are flexible with few assumptions, while the disadvantages are that they require a lot of data, are hard to interpret, and are computationally heavy.