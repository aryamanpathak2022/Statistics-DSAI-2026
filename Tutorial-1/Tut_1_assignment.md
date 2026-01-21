

# Assignment: E-Commerce Performance Analysis 


**Topic:** Introduction to NumPy, Pandas, and Matplotlib


### 1. The Scenario

You have just been hired as a **Junior Data Analyst** for a growing e-commerce retail company. Your manager has given you a raw dataset of recent sales and asked you to generate a performance report. She wants to know which product categories are doing well, how profits are distributed, and statistical summaries of the revenue.

### 2. The Dataset

You will be working with a CSV file named `superstore_sales.csv`.

* **Source:** [Sample Superstore Dataset on Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
* **Key Columns:** `Order Date`, `Category`, `Region`, `Sales`, `Quantity`, `Profit`.

---

### 3. The Tasks

#### Part A: Data Inspection & Cleaning (Pandas)

*Objective: Get comfortable loading and inspecting dataframes.*

1. **Load the Data:** Import pandas and load the `superstore_sales.csv` file into a DataFrame.
2. **First Look:** Display the first 5 rows and the last 5 rows of the dataset.
3. **Data Info:** Use `.info()` to check for missing values and data types. Are there any columns that need cleaning?
4. **Statistical Summary:** Use `.describe()` to see the quick statistical summary of the numerical columns (Sales, Profit, Quantity).

#### Part B: Statistical Analysis (NumPy)

*Objective: Use NumPy for mathematical operations on data arrays.*

1. **Array Conversion:** Convert the `Sales` column into a NumPy array named `sales_array`.
2. **Central Tendency:** Calculate the **Mean** and **Median** sales using NumPy functions. Compare them—is the mean higher than the median? What does that imply about the data (skewness)?
3. **Dispersion:** Calculate the **Standard Deviation** of the `Profit` column. This tells us how volatile our profits are.
4. **High Value Filters:** Use `np.where` or boolean indexing to count how many orders had `Sales` greater than **500**.

#### Part C: Business Insights (Pandas Manipulation)

*Objective: Grouping and filtering to answer business questions.*

1. **Category Analysis:** Group the data by `Category`. Calculate the **Total Sales** and **Total Profit** for each category. Which category is the most profitable?
2. **Regional Trends:** Which `Region` has the highest number of orders? (Hint: Use `value_counts()`).
3. **Loss Analysis:** Filter the dataframe to create a new dataframe called `loss_df` that only contains rows where `Profit` is negative (< 0). How many distinct orders resulted in a loss?

#### Part D: Visualization (Matplotlib)

*Objective: Visualizing the insights for the manager.*

1. **Sales Distribution:** Create a **Histogram** of the `Sales` column. Use 20 bins. (Tip: Since sales data is often skewed, you might want to limit the range to sales under 1000 for a clearer plot).
2. **Category Performance:** Create a **Bar Chart** showing *Total Sales* for each *Category*. Label your X and Y axes clearly.
3. **Correlation Check:** Create a **Scatter Plot** with `Sales` on the X-axis and `Profit` on the Y-axis. Is there a linear relationship? Do higher sales always mean higher profit?

---


---


