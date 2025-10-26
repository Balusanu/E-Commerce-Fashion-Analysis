# E-Commerce Women’s Fashion Sales Analysis & Automation

## 📌 Project Overview

This project involves **cleaning, analyzing, visualizing, and automating insights** from a large dataset of women’s fashion products. The dataset contains **30,000 products** covering a wide range of apparel and accessories.

The main objective is to **prepare the data**, **extract meaningful insights**, and **automate reporting** for business decisions.

---

## 👜 About the Dataset

The dataset consists of women’s fashion products with multiple categories and attributes.

### Categories Covered:

* Western Wear
* Indian Wear
* Perfumes & Fragrances
* Watches
* Nightwear

### Column Descriptions:

| Column Name   | Description                                                           |
| ------------- | --------------------------------------------------------------------- |
| **BrandName** | Brand or manufacturer of the product                                  |
| **Details**   | Descriptive details about the product (style, material, design, etc.) |
| **Size**      | Available sizes (e.g., S, M, L, XL)                                   |
| **MRP**       | Maximum Retail Price (before discount)                                |
| **SellPrice** | Selling Price after discounts                                         |
| **Category**  | Main product category (e.g., Western Wear, Watches)                   |

---

## 🛠 Libraries Used

* **NumPy** – for numerical operations
* **Pandas** – for data cleaning and manipulation
* **Matplotlib** – for visualizations
* **Seaborn** – for statistical plots

---

## ⚙ Steps Performed

1. **Importing libraries**
2. **Loading the dataset**
3. **Renaming columns properly**
4. **Ordering columns in the correct sequence**
5. **Extracting MRP and discount values**
6. **Cleaning category names** (removing unnecessary strings like `-Women`)
7. **Replacing string "Nan" with `np.nan`**
8. **Converting MRP, SellPrice, and Discount columns to float**
9. **Checking and removing duplicate records**
10. **Handling null values**

    * `Details` column dropped (low significance)
    * `Size` column dropped (inconsistent data)
    * `BrandName` nulls replaced with **Mode**
    * `Discount` nulls replaced with **Mean**
    * `MRP` & `SellPrice` nulls replaced with **Median**
11. **Data Analysis & Insights**

    * Top categories by number of products
    * Categories with highest total sales
    * Categories with highest & lowest average discounts
    * Most expensive product by category
    * Brands with highest sales, costliest products, and highest discounts
12. **Creating separate dataframes for each category**
13. **Exporting category-wise data**

---

## 📊 Key Insights

* **Duplicate Records:** 1,331 duplicates removed

* **Category Insights:**

  * Western Wear (9,962) and Indian Wear (9,858) cover ~2/3 of total products
  * Watches achieved **₹1.5 Crore** sales with only 1,725 products
  * Indian Wear has the **highest average discount**: 49.6%
  * Fragrance: 36% average discount
  * Watches: costliest product priced at **₹1.4 Lakh**

* **Brand Insights:**

  * Vastranand (Indian Wear) – highest total sales: ₹32 Lakhs
  * Versace, Tissot, Michael Kors – most expensive items
  * Gas (Indian Wear) – highest average discount

---

## 📂 Output

* Exported **separate CSV files** for each product category for further analysis or reporting.

---

## 🔗 Project Usage

1. Clone this repository:

```bash
git clone <repository-url>
```

2. Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn
```

3. Run the Jupyter Notebook or Python script to perform **data cleaning, analysis, and automation**.
4. Check the `exports` folder for category-wise CSV files.

---

## 📌 Conclusion

This project provides a **clean, structured dataset** with actionable insights on sales, discounts, and pricing. The exported data files allow **automation of reports**, helping stakeholders make informed decisions.

---

✅ **Next Steps / Future Work**

* Implement **interactive dashboards** in Power BI or Plotly
* Predict **sales trends** using machine learning
* Automate weekly/monthly **report generation**
