<p align="left"><img src="https://cdn-images-1.medium.com/max/184/1*2GDcaeYIx_bQAZLxWM4PsQ@2x.png"></p>

# Module 2 project: Data analytics of a Diamonds dataset

## **Objectives:**
Using __diamonds_train.csv__ dataset that can be found [here](https://www.kaggle.com/shivam2503/diamonds):

- Do an exploratory data analysis. The analysis was done using Jupyter, Pandas and libraries for plotting and is stores on  `data_analysis_report.ipynb` file, that holds the results of __Challenge 1__ + __Bonus Challenge__. 

- Create a dashboard using Tableau Public that can be found [here](https://public.tableau.com/profile/alvaru89#!/vizhome/Module2project/Dashboard1).

- Document the process in the `README.md` file you are reading.


## **Exploratory data analysis:**

The notebook includes the code used for:
 - Creation of descriptive statistics  such as max, min, mean, standard deviation, percentiles, correlations, etc.) and data types (integer, float, boolean, string, etc.).
 - Some basic charts in order to visually identify outliers, trends, correlations, completeness/void in the dataset, aggroupation/ at an early stage.


## **Dashboard and presentation:**

The dashboard is composed by 5 graphs:

<p align="center"><img src="images/dashboard.png"></p>

- "Precio vs Quilates y agrupados por Claridad" or "Price vs Carat, grouped by Clarity"

On this plot, we can easily see relationship between carat and price. Bigger diamonds are more expensive.
Also, a fan distribution can be noticed. The price of the small diamonds is relatively similar for all clarities but the clarity has an impact on bigger diamonds, translated in an increasing slope with increasing clarity. This means that for the same carat, the price of worse clarity is lower.

- "Variables de Precio vs Claridad" or "Price variables vs Clarity"

The plot intended to show the difference in price between clarity. However, it shows that diamonds with high prices can be found in all clarity sub-groups. This was unexpected because the clarity can be understood as a level of quality of the diamond and the most expensive diamonds should have the best clarity. 

Since we saw a relationship between price and carat and we were interested on the clarity-quality, which is unrelated to the weight, removing the effect of the carat seemed sensible. Therefore a new variable was created: 'price/carat'.
As expected, a better clarity can lead to an increase of the price/carat.

- "Prom. Precio vs Quilates y Corte" or "Average Price vs Carat and Cut"

The effect of the cut was studied on both price variables. The lines of the average price are basically overlaped, meaning that the cut has a negligible effect. The worst cut is slightly below than the orders, but this could well be because of the smaller amount of values relative to the other sub-groups and it may not be relevant enough.

- "Precio/Quilates agrupados por color" or "Price/Carat, grouped by color"

Again, the color has a similar 'fan'effect, meaning that smaller diamonds are not affected by the color but bigger diamonds are.
Comparing to clarity, the effect of color is less direct but still noticeable.


- "Precio/Quil. vs Color" or "Price/Carat vs Color"

This boxplot shows a high concentration of diamonds with Price/Carat below 5000 USD. This is consistent with the conclusion before, and hides the effect of color on price and price/carat on diamonds with better color.
By changing the filter to at least 8000USD, it is easier to identify the correlation.

## **Bonus Challenge: Hypothesis Testing**

The following hypothesis were tested using Stats module from Scipy library.

**Test 1 - one sample vs constant hypothesis test.** The aim is to test whether the prices in our sample are significantly different from 4000 USD. 

The test found significant difference to the mean value of 4000 USD.

**Test 2 - two independent samples.** The aim is to test several pair of "sub-groups" and look for signifcant difference.

- **Sub-Test 1:** Fair cut + color G vs. Fair cut + color I

- **Sub-Test 2:** Good cut + color E vs. Good cut + color F

- **Sub-Test 3:** Ideal cut + color D vs. Ideal cut + color E

- **Sub-Test 4:** Premium cut + color D vs. Premium cut + color E

- **Sub-Test 5:** Very Good cut + color I vs. Very Good cut + color J

- **Sub-Test 6:** All cuts + color D vs. All cuts + color E

The outcome of all tests was that none of the subsets was significantly different. The reason can be that the comparison is done between adjacent groups of colors. For example, when comparing color D (best color) to the color J (worst color), a significant difference was found.