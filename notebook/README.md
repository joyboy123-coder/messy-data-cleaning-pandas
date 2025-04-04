# 🧹 Data Cleaning Project (1000 Rows Dataset)

This project demonstrates how a raw, messy dataset containing 1000 rows was cleaned and transformed into a structured and usable format using **pandas** in Python. Below is a step-by-step explanation of how each part of the cleaning process was performed:

---

## 📥 1. Loading the Dataset

- The raw dataset was loaded using `pandas.read_csv()` by prompting the user to input the file path.
- The first few rows were inspected to understand the structure, formatting issues, and missing data.

---

## 🧼 2. Column Cleaning

- Column names were cleaned by converting them to **title case** and **stripping extra spaces** for consistency and readability.

---

## ✂️ 3. Removing Unwanted Rows

- The **last 10 rows** of the dataset were removed, likely because they were blank, irrelevant, or contained corrupt data.

---

## 👤 4. Cleaning the `Name` Column

- The `Name` column was converted to **title case** and stripped of any leading/trailing whitespace.
- The full name was then **split into `First Name` and `Last Name`**, assuming the first space separated them.
- The original `Name` column was dropped after the split.

---

## 📅 5. Cleaning the `Date` Column

- All dates were parsed into a proper `datetime` format using `pandas.to_datetime()` with error handling.
- For missing or invalid dates, a custom **date range starting from June 12, 2020** was generated and filled in every 2 days to maintain uniqueness and order.

---

## 🎂 6. Handling Missing Values in `Age`

- Non-numeric values in the `Age` column were coerced to NaN.
- Missing `Age` values were filled using **random sampling from existing non-null ages** in the dataset to ensure realistic imputation.
- Finally, all ages were converted to integers.

---

## 🏙️ 7. Cleaning the `City` Column

- City names were cleaned by converting to **title case** and removing any extra spaces for uniformity.

---

## 🧾 8. Final Column Arrangement

- The final dataset was reordered to include the following columns only:
  - `First Name`
  - `Last Name`
  - `Age`
  - `Date`
  - `City`

---

## 💾 9. Saving the Cleaned Dataset

- After completing all the cleaning steps, the final cleaned dataset was saved as a **new CSV file** using the `to_csv()` function.
- This ensures the cleaned version can be used independently from the raw file, preserving the transformation work.

---

## ✨ Summary

This project is a good example of a practical data cleaning pipeline where:
- Inconsistent casing, formatting, and NaNs were handled.
- Columns were properly structured and enriched.
- The final output was made analysis-ready with minimal assumptions.

