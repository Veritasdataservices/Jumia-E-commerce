
Q10 — Returns by Category (method & limitation)

Direct data: processed/orders_clean.csv shows 480 returned orders out of 5,000 total orders (9.60% overall).

Limitation: There is NO order_items table linking orders to products/SKUs. Therefore exact return rates per SKU/category cannot be computed from the available data.

Approximation performed: Returned orders were ALLOCATED to categories proportionally to each category's potential inventory revenue (unit_price × stock_quantity). This allocation is directional only and should be used for hypothesis generation, not as a definitive attribution.

Recommendation:
1. Obtain transaction-level order_items to compute true return rates by SKU/category.
2. Use the approximation to prioritize categories for immediate audit (inventory accuracy, product quality checks, and customer feedback review).
3. Cross-reference with return reasons and customer reviews (if available) to validate the approximation.

Files:
- processed/q10_returns_by_category_approx.csv
- charts_output/q10_returns_by_category_approx.png
