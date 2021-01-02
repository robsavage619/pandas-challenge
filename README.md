# Demographic and Purchasing Analysis (Video Games)

![Fantasy](Images/Fantasy.png)

---

![Visualization](Images/pandas_gif.gif "Notebook Walkthrough")

---

## Contact Information

Rob Savage 

rob.savage@me.com

[LinkedIn](https://www.linkedin.com/in/robsavage/)


[Tableau Public](https://public.tableau.com/profile/rob.savage)

---

## Project Description

The purpose of this project was to use provided data set that includes `Purchase ID`, `SN`, `Age`, `Gender`, `Item ID`, `Item Name`, and `Price` to analyze purchasing habits by demographics. 

---

## Tools Used

1. Python (Data Aggregation/Cleaning)

    - Pandas Library

2. NumPy (Calculations)

3. Github (Publishing of Results and Analysis)

4. Jupyter Notebook

---

## Steps 

1. Used `Python` to aggregate/clean data from the `purchase_data.csv` in the `Resources` folder with `Pandas`. 

    - Player Count was achieved by running a unique sort on the `SN` column due to the nature of the data that was unique to each user
    - A basic Purchasing Analysis was run calculating `Number of Unique Items`, `Average Price`, `Number of Purchases`, and `Total Revenue`
    - The Gender Demographics were tabulated by utilizing the `groupby` method in `Gender`, then running a unique count on those groups. The `Percentage of   Players` was calculated with value counts on that column
    - A Gender Purchasing Analysis was calculated using a combination of `groupby` along with a few mathematical calls in `mean`, `sum`, and `count`
    - The Age Demographics Analysis was calculated using `binning` to create groups for the age demos, then running unique counts on those associated screenames
    - Utilizing those very same bins, the same method from the Gender Purchasing Analysis was applied to get calculations for those age groups
    - To calculate the Top Spenders, I performed a `groupby` on the `SN` column, then ran a few mathematical calls in `mean`, `sum`, and `count`
    - The Most Popular Items were found by grouping the `Item ID` and `Item Name`, then running `mean`, `sum`, and `count`
    - Finally the Most Profitable Items was calculated by taking the data frame created in the previous step, then sorting the `Total Purchase Value`

---

## Analysis


1.) There is a surprising demographic gap in gender--84% of the unique players of HOP are male. There isn't a surprise that the majority are male, but more so that in 2020 we see such a large divide in the demo especially with female gamers becoming more prevalent in the market. 

2.) With basic knowledge of the economics and market trends of the gaming industry, with a total unique user pool of 576, the total revenue numbers of $2,379.77 are awfully low. The entire industry is making the shift towards microtransactions and these figures need to rise dramatically.

3.) The sweet spot for the game's marketing department is the 20-24 age range. Not only does it hold the largest player base, it has the highest average total purchase per person. There's a significant increase from 15-19 to 20-24, which is explained by the the presumed increase in disposable income. 

