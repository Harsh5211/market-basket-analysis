
# Market Basket Analysis Project

This project delivers a comprehensive **Market Basket Analysis** using point-of-sale and loyalty datasets to uncover customer purchasing patterns. It integrates EDA, clustering, and association rule mining to extract meaningful business insights and support data-driven marketing strategies.

---

##  Datasets Used

- **POS Data** Customer transactions (items bought, dates, quantities).
- **Loyalty Data** – Customer demographics including number of children and household info.
- **Barcodes Data** – Item identifiers for mapping.
- **Product Taxonomy** – Category descriptions for interpretability.

---

## Project Workflow

### 1.  Data Preparation
- Checked and treated null values
- Merged datasets using barcode and card IDs
- Enhanced readability with product category names

### 2.  Exploratory Data Analysis (EDA)
- Analyzed top-selling product categories
- Investigated revenue patterns by household size and gender
- Identified customer preferences by segment

### 3.  Association Rule Mining (Apriori Algorithm)
Key metrics used:
- **Support**: Frequency of item combinations
- **Confidence**: Probability of co-occurrence
- **Lift**: Strength of association compared to random chance

#### Top Insights:
- `pasta → spaghetti` (Confidence: 20.59%, Lift: 2.89)
- `Sweet & Savoury Base → poweder` (Lift: 2.39)
- `no sugar → instant coffee` (Lift: 2.02)
- Avoid `LIMITED DURATION → poweder` (Lift: 0.90 – weak)

---

## Clustering Analysis
- **KMeans Clustering** used to segment customers/products
- Segments reflect unique purchase behaviors and item preferences
- Aids in targeting and personalization

---

##  Business Recommendations

- Promote high-lift pairs through **combo offers** or **cross-selling**
- Bundle items like **pasta & spaghetti**, **no sugar & instant coffee**
- Ignore weak or negative associations in promotions
- Leverage loyalty segments for tailored campaigns

---

## Conclusion

Market Basket Analysis empowers retailers to:
- Understand **co-purchase behavior**
- Drive **personalized promotions**
- Increase **basket value and customer retention**

This notebook provides a practical, end-to-end implementation of MBA with real-world retail data.

---

**Author**: Mr.Harsh R Thakkar  
**Toolkits**: `pandas`, `mlxtend`, `scikit-learn`, `matplotlib`, `seaborn`  
**License**: MIT

