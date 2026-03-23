#  R Programming — Assignment 

Resource - https://www.w3schools.com/r/

## Instructions

- Attempt **all** questions.
- Write clean, well-commented R code.
- Each code block should run without errors.
- Use `print()` to display all outputs clearly.

---

## Section A — Variables, Vectors & Data Frames

### Question 1

Create the following variables and print them:

- A **character** variable called `city` storing the name of your hometown.
- A **numeric** variable called `population` storing an approximate population of that city.
- A **logical** variable called `is_capital` storing whether or not it is a state capital.

After creating them, use the `class()` function to print the data type of each variable.

---

### Question 2

Create a numeric vector called `monthly_sales` with the following values:

```
12000, 15400, 9800, 17600, 14200, 16800
```

Using R's built-in functions, calculate and print:

1. The **total** sales (use `sum()`)
2. The **average** monthly sales (use `mean()`)
3. The **highest** sales month (use `max()`)
4. The **lowest** sales month (use `min()`)

---

### Question 3

Create a Data Frame called `class_records` with the following data for **5 students**:

| Column | Type | Sample Values |
|---|---|---|
| `StudentName` | Character | Names of 5 students |
| `Marks` | Numeric | Any 5 scores out of 100 |
| `Passed` | Logical | TRUE if Marks >= 40, else FALSE |

After creating the data frame:

1. Print the **entire** data frame.
2. Print **only** the `Marks` column.
3. Use `subset()` to print only the rows where the student has **passed**.

---

## Section B — Lists, Control Flow & Functions

### Question 4

Create a **list** called `my_profile` that stores the following about yourself:

- `name` — your name (Character)
- `age` — your age (Numeric)
- `hobbies` — at least 3 hobbies (a Character vector)
- `is_student` — whether you are currently a student (Logical)

Print the entire list, and then print **only** your hobbies using the `$` operator.

---

### Question 5

Write an **if-else** statement for a grading system.

Create a variable called `score` and assign it any value between 0 and 100. Write logic that prints:

- `"Grade: A"` — if score is 90 or above
- `"Grade: B"` — if score is 75 or above
- `"Grade: C"` — if score is 60 or above
- `"Grade: D"` — if score is 40 or above
- `"Grade: F"` — if score is below 40

---

### Question 6

Write a **for loop** that iterates over the `monthly_sales` vector you created in Question 2.

For each value, print a message in this format:

```
Month 1 sales: 12000
Month 2 sales: 15400
...
```

*Hint: Use `paste()` to combine text and numbers.*

---

### Question 7

Write a **custom function** called `bmi_calculator` that:

- Takes two arguments: `weight_kg` and `height_m`
- Calculates BMI using the formula: **BMI = weight / (height²)**
- Returns the BMI value (rounded to 2 decimal places using `round()`)

Test your function with at least **two different** sets of values and print the results.

---

## Section C — Data Exploration

### Question 8

Use R's built-in `airquality` dataset for this question. Load it with `data(airquality)`.

1. Print the **first 8 rows** using `head()`.
2. Use `summary()` to display descriptive statistics for the dataset.
3. The `Ozone` column contains missing (`NA`) values. Calculate the **mean Ozone level**, making sure to properly handle the `NA` values.
4. Use `subset()` to create a new data frame called `hot_days` containing only the rows where `Temp` is greater than **90**.
5. Print `hot_days` and state how many such days exist (use `nrow()`).

---


