# Gift Shop Sales & Customer Dataset

This project contains a relational dataset tracking orders, products, and customer information for a specialized gift shop. The data is structured to allow for analysis of seasonal trends (like Diwali, Holi, and Valentine's Day) and customer purchasing behavior across different Indian cities.

## 📂 File Structure

The dataset is split into three primary tables:

| File | Description | Key Columns |
| :--- | :--- | :--- |
| `customers.csv` | Personal details of registered shoppers. | `Customer_ID`, `City`, `Gender` |
| `products.csv` | Catalog of items available for sale. | `Product_ID`, `Category`, `Price (INR)` |
| `orders.csv` | Transactional records linking customers to products. | `Order_ID`, `Order_Date`, `Location` |

---

## 📊 Data Dictionary

### 1. Customers Table
Contains demographic information for 100+ customers.
* **Customer_ID**: Unique identifier (Primary Key).
* **Name / Email / Contact**: Personal contact details.
* **City / Address**: Geographic location for shipping analysis.

### 2. Products Table
A list of gift items categorized by type and intended occasion.
* **Product_ID**: Unique identifier (Primary Key).
* **Category**: Includes Soft Toys, Plants, Colors, Sweets, Cake, Mugs, etc.
* **Price (INR)**: The cost of a single unit.
* **Occasion**: Suggested event (e.g., Anniversary, Raksha Bandhan).

### 3. Orders Table
The "Bridge" table that connects customers to the products they bought.
* **Order_ID**: Unique transaction ID.
* **Quantity**: Number of items purchased.
* **Order_Date / Delivery_Date**: Timeline of the transaction.
* **Occasion**: The specific event the order was placed for.

---

## 🛠 How to Use This Data

### For Excel Users
1.  Open `orders.csv` in Excel.
2.  Use **VLOOKUP** or **XLOOKUP** to pull Product Names from `products.csv` using the `Product_ID`.
3.  Pull Customer Names from `customers.csv` using the `Customer_ID`.
4.  Create **Pivot Tables** to see which `Occasion` generates the most revenue.
## 💡 Key Insights

Based on an analysis of the current dataset, here are the primary trends and findings:

### 1. High-Demand Occasions
The data shows distinct sales peaks aligned with major cultural and personal events:
* **Cultural Festivals:** Festivals like **Diwali**, **Holi**, and **Raksha Bandhan** drive significant transaction volume.
* **Personal Milestones:** **Anniversaries** and **Birthdays** are consistent year-round contributors to total sales.
* **Seasonal Peaks:** **Valentine's Day** shows a concentrated spike in specific categories like Mugs, Plants, and Soft Toys.

### 2. Top Performing Product Categories
* **Gift Essentials:** Categories such as **Sweets**, **Cake**, and **Flowers** are frequently purchased across almost all occasions[cite: 21, 23].
* **Keepsakes:** **Mugs** and **Soft Toys** are top choices for Valentine's Day and personal celebrations.
* **Niche Interests:** **Plants** and **Colors** (specifically for Holi) represent growing segments in the gift catalog.

### 3. Geographical Distribution
* Sales are widely distributed across diverse Indian cities, with notable activity in locations like **Jaipur**, **Bardhaman**, **Bilaspur**, and **Guwahati**.
* Shipping data reveals a mix of Tier 1 and Tier 2 cities, indicating a broad market reach[cite: 1, 25].

### 4. Customer Demographics
* The customer base is nearly evenly split between **Male** and **Female** shoppers, though purchasing preferences vary by category.
* There is a high rate of repeat customers (linked by `Customer_ID`), suggesting strong brand loyalty for recurring annual events[cite: 1, 48].
