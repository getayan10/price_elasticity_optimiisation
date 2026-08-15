# Price Elasticity Optimiisation
An econometric price elasticity and revenue optimization framework built in Python. It features log OLS regression models to analyze product demand sensitivity, control for promotional effects, and simulate optimal pricing (P*) for revenue lift.

Project Overview
This project applies econometric modeling and constant-elasticity demand functions to analyze retail pricing data. By identifying price elasticity of demand across product categories, the pipeline simulates price adjustments (-25% to +25%) to discover optimal price points ($P^*$) that maximize overall revenue.

Technical Architecture & Pipeline
1. Data Preprocessing & EDA: Cleaned transactional records, handled zero-volume days, and performed log transformations.
2. Econometric Modeling: Fitted Log-Log Ordinary Least Squares (OLS) regression models using `statsmodels` to extract category-level price elasticity coefficients ($\beta_1$). Controlled for freight pricing, weekends, and holidays.
3. Revenue Simulation: Implemented a non-linear optimization function to predict demand shifts and project total revenue at incremental price steps.

Key Results & Business Recommendations
Elastic Categories: High price sensitivity. Lowering prices drives disproportionate unit volume growth, increasing total revenue.
Inelastic Categories: Low price sensitivity. Raising prices increases per-unit profit margins with minimal drop in sales volume.
**Projected Impact:** Implementing optimal prices yields a **projected revenue lift across target categories**.

## File Structure
price-elasticity-optimization/
├── retail_price.csv
├── price_elasticity_processed.csv
├── category_elasticity_results.csv
├── price_optimization_summary.csv
├── executive_summary_dashboard.png
├── price_elasticity_analysis.ipynb
└── README.md
