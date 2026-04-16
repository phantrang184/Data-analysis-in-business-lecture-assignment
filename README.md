# Data-analysis-in-business-lecture-assignment
Data analysis lecture: Mainly about Basic methods in business data analysis, including descriptive, predictive, and prescriptive analytics.
## 1. Factors affect clothing stores profit:
Load dataset from Clothing.csv
a. Executive Summary:
The analysis evaluates a dataset of 400 clothing stores to identify the drivers of total sales (tsales) and optimize operational efficiency. Key variables include store size, labor hours, and margin.

b. Key Analytical Insights:

- Labor as the Primary Driver: There is a high correlation between total sales and labor-related variables (hoursw, hourspw, and nfull).
--> Labor hours are the strongest predictors of revenue, but high VIF (Multicollinearity) scores suggest these variables are deeply interconnected.

- Inventory Optimization (ABC Analysis):

  Group A (20% items, 80% revenue): Focus on tight forecasting and rapid replenishment.

  Group B (30% items, 25% revenue): Moderate monitoring.

  Group C (50% items, 10% revenue): Liquidate or transfer these items to avoid high holding costs.

- Store Size Efficiency: The optimal store size is identified between 150-350 m². Beyond this, the incremental cost of rent may diminish overall profitability unless sales per square meter increase proportionally.
- Customer Journey & Layout: Using an arc-shaped shelf arrangement encourages customers to walk through the entire store. Placing high-margin or new arrivals in the center/back and best-sellers near the entrance maximizes "impulse buying" opportunities.

c. Strategic Recommendations
- Staffing: Align labor hours strictly with store size and peak traffic periods.
- Margin Management: Review products with low margins for potential removal or conversion into promotional "loss leaders" to drive foot traffic.
- Layout: Position best-selling items at the entrance to attract customers, while placing high-margin items in the middle to end of the store journey.

## 2. Delivery Performance Analytics

This project develops a data analytics framework for examining shipment performance in a logistics dataset. The study combines descriptive statistics, exploratory visualization, and multivariate data analysis in Python to identify patterns affecting on-time delivery outcomes and customer service efficiency.
Load dataset from Train.csv.

### 2.1. Problem description:

- Each observation corresponds to one delivered order, characterized by logistics, product, and customer-related attributes.

- The dataset contains:
  - Observations: 10,999 shipment records
  - Target variable: Delivery status (Reached.on.Time_Y.N)
  - Predictor groups:
    - Warehouse information
    - Shipment mode
    - Customer service interaction
    - Product characteristics
    - Purchase history
    - Pricing and discount variables

- The project addresses three analytical objectives:
  - Part 1 – Descriptive Statistical Analysis: summarize the central tendency, dispersion, and distribution of all major variables;
  - Part 2 – Data Visualization: explore trends, correlations, and categorical patterns through graphical representation;
  - Part 3 – Data Mining Analysis: identify relationships between explanatory variables and delivery outcomes, highlighting factors associated with delayed shipments.
### 2.2. Data and implementation structure:

The analysis uses the file Train.csv, where each row represents one shipment transaction and columns define shipment attributes.
### 2.3. Descriptive analysis framework (Part 1):

The first phase evaluates statistical properties of both numerical and categorical variables. The following measures are computed:
- Mean
- Median
- Standard deviation
- Minimum / Maximum
- Quartiles

This stage provides an overview of shipment behavior and reveals skewness, concentration ranges, and unusual values.

### 2.4. Visualization analysis (Part 2):

The second phase applies graphical tools to detect patterns and compare distributions. Typical visual outputs include:
- Histogram plots for numerical distributions
- Boxplots for outlier detection
- Countplots for categorical frequency comparison
- Correlation heatmaps among quantitative variables
- Bar charts comparing delayed vs on-time deliveries across shipment categories

These visualizations help identify operational trends:
- Orders shipped via Ship mode account for the largest share of delayed deliveries, implying that this transportation channel may face higher congestion or operational inefficiencies.
- Certain warehouse blocks consistently show higher late-delivery frequency, suggesting uneven warehouse performance across locations.
- Heavier packages appear more likely to experience delays, indicating that package weight may increase fulfillment and transportation complexity.
- Higher discount orders tend to cluster more in delayed deliveries, which may reflect demand surges caused by promotions putting pressure on logistics capacity.
### 2.5. Exploratory data mining analysis (Part 3):
The third phase investigates associations between predictors and delivery performance. Analytical focus includes:
- Comparing delayed and on-time groups across all major variables;
- Detecting significant behavioral differences in customer purchase history;
- Evaluating how discount size affects shipment punctuality;
- Examining warehouse and shipment mode influence on delivery success.

Business Implication:
- Among the three transportation modes, ship transport has the highest on-time delivery rate. Therefore, the remaining shipping methods should be reviewed carefully, and products should be categorized according to the most suitable transportation mode to achieve the highest delivery accuracy.
- Warehouse optimization: All warehouse blocks currently show a similar on-time delivery rate of around 60%. In the long term, the company may consider reducing redundant warehouses or relocating warehouse positions strategically to improve the on-time delivery rate to 80%.
- Adjust shipment mode by product type: Products should be classified based on characteristics such as perishability, urgency, and delivery distance, then assigned to the most appropriate transportation method.
- Improve employee performance: Employee training should be expanded, and a “carrot and stick” incentive system may be applied to enhance delivery efficiency. This can be particularly effective when employees become less attentive due to low-value orders.
- Set higher standards for partners: Stricter performance requirements should be established for warehouse and shipment partners. Partner screening should be conducted carefully before collaboration, and service-level agreements must clearly define expectations. This can improve accountability and operational focus.
- Optimize order allocation by weight: Orders should be arranged and distributed more efficiently according to shipment weight to reduce transportation time and improve logistics flow.
- Prioritize loyal customers
- Personalize delivery services


