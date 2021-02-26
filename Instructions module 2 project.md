<p align="left"><img src="https://cdn-images-1.medium.com/max/184/1*2GDcaeYIx_bQAZLxWM4PsQ@2x.png"></p>

# __ih_datamadpt0420_project_m2__

![Image](https://github.com/potacho/ih_datamadpt1120_project_m2/blob/master/images/visuals.jpg)

Data analytics is oftentimes referred to as business intelligence, BI development, or product analytics. However, that is just the tip of the iceberg since the data analytics process includes activities such as data formation/creation, data cleansing, exploratory data analysis (especially this part), feature engineering, and interpretation of suggestions/predictions/results derived from advanced modelling analysis (i.e.: Machine Learning).

For this project you will perform some of these activities in order to analyse the __diamonds_train.csv__ dataset. 



---



## **Deliverables:**

A GitHub repository, preferably named: __ih_datamadpt0420_project_m2__, including:

- `data_analysis_report.ipynb` file that holds the results of __Challenge 1__ + __Bonus Challenge__. 

- `Tableau Public Dashboard` including your dashboard proposal (__Challenge 2__).

- `README.md` file explaining the job done, your main conclusions and the __link to your Tableau Public Dashboard__. You may find more info of how to build a README file [here](https://github.com/potacho/data-project-template/blob/master/README.md).



---



## **Presentation:**

- __Time:__ 3 minutes sharp.
- __Content:__ explain why your dashboard funtionalities are the best for getting meaningful data insights. Support your arguments on the conclusions obtained from the __exploratory analysis__. Conclude your pitch telling us (_in one sentence_) the most important insight (_under your criteria_) you've extracted.

<p align="center"><img src="https://media.giphy.com/media/1Ygis29YXMS35cW90I/giphy.gif"></p>


> __IMPORTANT NOTE:__ You only need your Dashboard for the presentation (no Jupyter, no PowerPoint/Canva)



---



## __Challenge 1: Exploratory Data Visualization Charts and Summary Statistics__

The goal of this challenge is to build an __exploratory data analysis report__ in order to gain initial insight on our diamonds dataset. Your notebook must include:

- Summary statistics including descriptive statistics (max, min, mean, standard deviation, percentiles, correlations, etc.) and data types (integer, float, boolean, string, etc.).
- Data visualizations charts in order to capture a large amount of data all at once in a clear and concise manner (Box Plots, Histograms, Bar Plots, Scatter Plots, Correlation Matrix, etc.).

<p align="center"><img src="https://media.giphy.com/media/iP1qEUE7VKhLq/giphy.gif"></p>

> **IMPORTANT NOTE:** You may use any tool that you find more convenient in order to provide the requested output. 



---



## **Challenge 2: Tableau Data Dashboard**

Dashboards are powerful tools for communicating important information __at-a-glance__. The goal of this challenge is to build a data dashboard using our diamonds dataset that will help the final user (i.e.: yourself) to perform better during _Module 3 project (Kaggle Competition)_. 

> __Tip:__ you should first considerate which data and which indicators should be put on the dashboard. Then, decompose the key indicators from multiple dimensions. 

<p align="center"><img src="https://media.giphy.com/media/l46Cy1rHbQ92uuLXa/giphy.gif"></p>


A data dashboard is not exactly a sequential set of descriptive charts like those you have built in challenge 1. Instead, a data dashboard should be __a single interactive interface built around a specific objetive and which components are logically arranged in order to provide data relevant insights effectively__. Therefore, bear in mind the main objective of the competition: _understand the relationship between diamonds attributes (features) or group of attributes, and its price_.



--- 



## **Bonus Challenge: Hypothesis Testing**

<p align="center"><img src="https://github.com/potacho/ih_datamadpt1120_project_m2/blob/master/images/htesting.jpg"></p>

We might want to know if our sample and sub-samples are representative of diamonds in general. Moreover, we might want to reach some conclusions about the influence of certain diamonds features in their price. In that sense, we propose you to perform two statistical tests:

**Test 1 - one sample vs constant hypothesis test.** We know from the available literature that diamonds average price rounds about 4000 USD. The aim is to test whether the prices in our sample are significantly different from the literature value. Give some conclusions about the implications of your test results.

**Test 2 - two independent samples.** Our sample includes diamonds with different features (carat, cut, color clarity, etc.). It seems clear that the carat plays an important role in price. However, it's not that clear whether the prices of some "sub-groups" are significantly different from each other. These are the "sub-groups" that you might feel suspicious about it:

- **Sub-Test 1:** Fair cut + color G vs. Fair cut + color I

- **Sub-Test 2:** Good cut + color E vs. Good cut + color F

- **Sub-Test 3:** Ideal cut + color D vs. Ideal cut + color E

- **Sub-Test 4:** Premium cut + color D vs. Premium cut + color E

- **Sub-Test 5:** Very Good cut + color I vs. Very Good cut + color J

- **Sub-Test 6:** All cuts + color D vs. All cuts + color E

<p align="center"><img src="https://media.giphy.com/media/26vUAAwkzAMnBj9x6/giphy.gif"></p>

> __IMPORTANT NOTE:__ Remember to also include your conclusions about the implications of your test results and all metrics involved (e.g.: samples size).

---

## **References:**

- [Visual Analysis Best Practices](https://github.com/potacho/ih_datamadpt1120_project_m2/blob/master/images/visual-analysis-guidebook.pdf)

- [Financial Times Visual Vocabulary](https://github.com/ft-interactive/chart-doctor/tree/master/visual-vocabulary)

- [Matplotlib](https://matplotlib.org/)

- [Pandas Visualization](https://pandas.pydata.org/pandas-docs/stable/user_guide/visualization.html)

- [Seaborn](https://seaborn.pydata.org/)

- [Introducing plotly express](https://medium.com/plotly/introducing-plotly-express-808df010143d)

- [Tableau Public](https://public.tableau.com/)

- [Tableau Viz of the Day](https://public.tableau.com/es-es/gallery/?tab=viz-of-the-day&type=viz-of-the-day)

- [Statistical functions (scipy.stats)](https://docs.scipy.org/doc/scipy/reference/stats.html)

- [Two-sample one-tailed t-test with Scipy](https://stackoverflow.com/questions/15984221/how-to-perform-two-sample-one-tailed-t-test-with-numpy-scipy)
