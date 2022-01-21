# Cora Wagner

## What:
The filter tool allows you to easily clean data within Excel. You can quickly remove excess data that does not work for your research and focalize the data you want to continue looking at.

## Why:
Someone may choose to use the filter tool when they are working with very large data sets. When there is an abundance of data entries, it becomes time consuming to clean it. Using the filter tool makes it quick and easy to clean a large data set.

## How:
### Filter Button
The first set of data shows the exam scores for students in various studies showing the possible effect of home life and study habits. You can find a copy of the data set through [GitHub](https://github.com/CoraWagner/Filter/blob/15c1c21ab73d47d9e0e35ea4782ee3e8f8cea992/StudentsPerformance.csv).

#### Step 1: Data -> Filter
To use the filter, select a cell with data in it and click on the **Data** tab at the top of the Excel window.

![Filter Tool Location - Image 1](Data.png)

Then find the **Sort & Filter** subsection and select the **Filter** button.

![Filter Tool Location - Image 2](Filter.png)

Once you have clicked the **Filter** button, dropdown arrows will appear beside each heading cell.

![Name Dropdown Arrow](TestPreparationDropdown.png)

#### Step 2: Select Category and Set Filter
Each dropdown menu will look like this. It will give you an option to select all, or the ability to select each individual item in the category. In my example image there are only two items to choose from.

![Category Filter](TestPreparationSelection.png)

For the filtered data set pictured below I chose to focus on female student who have free/reduced lunch, completed the study course, and had a math score of 80 or higher. By choosing the different filters I was able to focus on 5 entries out of the 1,000 original entries.

![Filtered Data Set](Female_FreeLunch_Studied_80-100MathScore.png)

When using the dropdown menus, you can filter as little or as many categories as you would like. 

### Filter Equation
The next data set is a collection of cereals and the dietary statistics that pertain to a serving of each cereal. You can find a copy of the data set through [GitHub](https://github.com/CoraWagner/Filter/blob/64398241e4bf459fe211d29a0dfd6b7b0c8fe05b/cereal.csv). 

#### Single Criteria:
Click on the cell you would like the new table to populate in.

Type `=FILTER(A1:P46,J1:J46>=10,"")` into the Formula Bar.

![Filtered Using Equation Single Criteria](EquationFilter1.png)

This formula will return a table that has filtered out all data entries that contain 10 or less grams of sugar per serving.

#### Multiple Criteria:
Click on the cell you would like the new table to populate in.

Type `=FILTER(A1:P46,(J1:J46>=10)*(D1:D46>110),"")` into the Formula Bar.

![Filtered Using Equations Multiple Criteria](MultipleCriteria.png)

This formula will return a table that has filtered out all data entries that contain 10 or less grams of sugar **AND** have 110 or less calories per serving.

## Referenced Work
Exam scores data set on [Kaggle](https://www.kaggle.com/spscientist/students-performance-in-exams)

Cereal data set on [Kaggle](https://www.kaggle.com/crawford/80-cereals/version/2)

More information about the filter tool at [Microsoft Support](https://support.microsoft.com/en-us/office/filter-function-f4f7cb66-82eb-4767-8f7c-4877ad80c759)
