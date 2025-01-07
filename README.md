# Market Basket Analysis for Cross-Category Purchase Patterns
This project focuses on uncovering cross-category purchase patterns through **Market Basket Analysis (MBA)** to optimize bundling strategies, enhance sales, and improve marketing decisions.

---

## **Overview**
The dataset contains over **540,000 transactions** from a UK-based online retailer between **December 2010 and September 2011**, sourced from the [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/dataset/352/online+retail). It includes transaction-level details such as product descriptions, quantities, and customer IDs.

**Research Questions**:
1. How can we identify product bundles that maximize customer purchases and Average Order Value (AOV)?
2. What insights can be derived from high-lift associations in purchasing patterns?

---

### **Data Characteristics**
- **InvoiceNo**: Unique transaction ID.
- **Description**: Product name.
- **Quantity**: Number of items per transaction.
- **UnitPrice**: Price per unit.
- **CustomerID**: Unique customer ID.
- **Country**: Customer's country of residence.

### **Exploratory Analysis**
- **Customer Distribution**: ~87% of sales are from UK customers.
- **Price Insights**: The average product price is £3.90, with the highest-priced item at £650.
- **Seasonality**: Peak sales occur during the holiday season, with significant cancellations identified in December 2011.

### **Market Basket Analysis (MBA)**
#### **Level I - Product-Based Analysis**
- **Sparse Matrix Creation**: Generated a sparse matrix representing baskets of purchased items.
- **Scope Thresholds**: Experimented with minimum support thresholds (e.g., 0.02) to identify significant associations.

#### **Level II - Category-Based Analysis**
- **Categorization Techniques**:
  - Attempted clustering with Word2Vec and K-means but opted for keyword-based categorization for simplicity.
  - Keywords (e.g., "cake," "bag") matched with product descriptions for clustering.
- **Lift Analysis**:
  - High-lift product pairs (e.g., "paint" → "decoration") identified opportunities for cross-promotion.
  - Heatmaps visualized strong associations between product categories.

---

## **Key Insights**
1. **High-Lift Pairings**:
   - Examples: "Cake" and "Pink Polkadot," "Cup" and "Bowl."
   - Suggest valuable cross-selling opportunities.
2. **Category-Based Marketing**:
   - Related items (e.g., kitchen and decor) show high associations, enabling targeted campaigns.
3. **Store Layout Optimization**:
   - Position high-association items together to boost sales.
4. **Cross-Promotion Potential**:
   - Bundle frequently purchased items with discounts to increase AOV.

---

## **Recommendations**
1. **Cross-Promotion and Bundling**:
- Create bundles for high-lift pairs (e.g., "Paint & Decorations") and offer discounts to encourage multi-item purchases.

2. **Product Placement Optimization**:
- Highlight "Frequently Bought Together" items prominently on product pages.
- Use A/B testing to determine the most effective placement strategies.

3. **Inventory Management**:
- Automate reordering for popular product pairs to ensure availability during peak demand.


