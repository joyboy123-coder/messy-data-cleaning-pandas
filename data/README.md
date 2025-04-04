## 📁 Folder Structure & File Paths 🗂️

Let's break down how your data flows through this project, from raw messiness to clean perfection 🧹✨:

---

### 🔹 `data/raw_data/raw_data_1000_rows.csv` 🐍📊

- 📦 This is your **raw messy dataset** containing **1000 rows** of unstructured data.
- 🧩 It includes:
  - Inconsistent formatting 😵
  - Missing values ❌
  - Mixed date formats 📆
  - Untidy names and city names 🏙️
- 🛠️ This is the **starting point** of your cleaning pipeline.

---

### 🔹 `data/cleaned_data/cleaned_data_sample.csv` 🧼✅

- 📁 This file is **empty at the beginning**.
- 📌 During the script execution, you’ll be prompted to **copy its path** using the `input()` function.
- 📥 After cleaning, your cleaned dataset will be saved here using `.to_csv()` — turning chaos into a **clean, structured table**.
- 📊 Perfect for visualizations, analytics, or reporting.

---

### 🔄 Workflow Summary 🔍

1. 🚀 Load the raw dataset from `raw_data_1000_rows.csv`.
2. 🧹 Perform cleaning: fix name formats, date parsing, age imputations, and city standardization.
3. 💾 Save the cleaned DataFrame to `cleaned_data_sample.csv`.

---

✅ **After running the project**, check the `cleaned_data` folder to see your polished dataset — clean, consistent, and ready to shine 🌟📈!

