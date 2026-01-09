# Results

## Business Motivation and Financial Insight

As an OSAT company, Amkor Technology’s profitability is fundamentally driven by how effectively it converts invested capital into economic returns. Packaging and testing operations are highly capital- and labor-intensive, making capital efficiency a critical determinant of long-term value creation. For this reason, this project focuses on forecasting the **ROIC–WACC spread**, a metric that captures true economic profit rather than accounting profit.

**ROIC–WACC Spread Interpretation**

- **ROIC (Return on Invested Capital):** Measures how efficiently capital is converted into operating profit.  
- **WACC (Weighted Average Cost of Capital):** Represents the required return demanded by investors and lenders.  
- **Spread = ROIC – WACC**

| Spread Condition | Interpretation | Business Implication |
|------------------|----------------|----------------------|
| > 0 | Returns exceed cost of capital | Value creation |
| = 0 | Returns equal cost of capital | Break-even |
| < 0 | Returns below cost of capital | Value destruction |

The spread therefore serves as a forward-looking indicator of strategic health and capital allocation effectiveness.

---

## Model Results Overview

### Predictive Performance (Test Set)

- **RMSE:** 3.14  
- **MAE:** 2.74  
- **R²:** 0.64  
- **Directional Accuracy:** 71%  

The model explains approximately 64% of the variance in the ROIC–WACC spread and correctly predicts the direction of change in roughly 7 out of 10 quarters, which is strong performance given the small sample size and cyclical nature of semiconductor financial data.

*(insert graph1.jpg)*

---

## Forecast Insights and Visualization

The forecast projects the ROIC–WACC spread for the next 10 quarters. A key insight from the visualization is the **zero-crossing point**, where the spread transitions from negative to positive.

*(insert graph2.jpg)*

### Key Findings

- All modeled scenarios (optimistic, base, pessimistic) cross above zero by **mid-to-late 2026**.  
- This suggests a recovery in capital efficiency and a shift from value destruction to value creation within a 1–1.5 year horizon.  

---

## Business Interpretation of ROIC–WACC Outcomes

### When Spread < 0 (ROIC < WACC)

The firm is destroying shareholder value.

**Recommended Actions**
- Delay or pause large capital expenditures and facility expansions.  
- Optimize capacity utilization at existing sites.  
- Review underperforming customer contracts or product lines.  
- Reduce leverage or renegotiate financing to lower WACC.  

*Example:* If spreads remain negative, Amkor may postpone new capacity investments in emerging regions and focus on yield improvement and automation at current facilities.

---

### When Spread > 0 (ROIC > WACC)

The firm is creating shareholder value.

**Recommended Actions**
- Invest in advanced packaging technologies (2.5D/3D IC, SiP).  
- Expand capacity in high-demand regions.  
- Increase R&D spending to strengthen competitive differentiation.  
- Pursue long-term customer partnerships or strategic M&A.

*Example:* With spreads projected to turn positive by mid-2026, Amkor could confidently plan expansion and long-term customer commitments beginning that period.

---

## Statistical Validation

- **Shapiro–Wilk Test (p = 0.16):** Residuals are approximately normally distributed, indicating unbiased errors.  
- **Durbin–Watson (0.19):** Positive autocorrelation remains, suggesting the model may lag during sharp turning points.  

Despite some temporal dependence, the model is statistically stable and well-suited for strategic, medium-term planning rather than short-term tactical forecasting.

---

## Revenue Model Results and Drivers

In addition to ROIC–WACC forecasting, a revenue prediction model was developed. Feature importance analysis reveals the following key drivers:

*(insert graph3.jpg)*

### Top Revenue Drivers and Interpretation

1. **Net Debt (lagged 4 quarters):** Indicates debt-funded investment cycles lead revenue growth.  
2. **Return on Assets (ROA):** Higher asset efficiency translates into stronger future revenue.  
3. **SOXX Index:** Confirms strong alignment with the broader semiconductor cycle.  
4. **Gold Prices:** Acts as a macro risk indicator affecting demand sentiment.  
5. **Materials Expenses (lagged):** Serves as a leading indicator of upcoming production ramps.  
6. **Communications Segment:** Core demand driver tied to networking and mobile chips.  
7. **Computing Segment:** Reflects AI, server, and high-performance computing demand.  

**Executive Summary Insight:**  
Amkor’s revenue is primarily driven by investment cycles, operational efficiency, and industry-wide semiconductor demand. Leverage and material spending act as leading indicators, while market and segment exposure shape revenue volatility.

---

## Strategic Takeaway

The combined forecasting framework indicates that **2025 should emphasize cost control and operational optimization**, while **2026–2027 presents a window for growth-oriented capital deployment**. The model provides quantitative support for timing strategic investments, enabling Amkor to transition from defensive capital management to expansion with greater confidence.
