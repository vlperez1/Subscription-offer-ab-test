# Subscription-offer-ab-test
A statistical A/B testing project analyzing the impact of different subscription offers on user conversion rates. This project uses descriptive statistics, hypothesis testing, and ANOVA to identify which offer performs best and provides data-driven recommendations for optimizing subscription revenue.

---

## Project Overview

The goal of this project is to evaluate multiple subscription offers (e.g., a baseline monthly plan, a discounted monthly plan, and a discounted annual plan) and determine which variant yields the highest conversion rate and revenue potential.

---

### 1. Problem Definition
- Define the business question: *Which subscription offer leads to higher user conversion and revenue?*
- Formulated null and alternative hypothesis for:
  - Overall conversion rate differences between offers.
  - Secondary metrics (time on page, click-through rate, etc.)
 
### 2. Data Collection & Loading
- Import the A/B testing dataset (marketing experiement data from Kaggle).
- Load the dat into a Jupyter Notebook using 'pandas'.
- Inspect scehma, datatypes, and basic structure

### 3. Data Cleaning & Preparation
- Handle missing or inconsistent values
- Filter out test users, bots or invalid sessions if necessary
- Create or format key columns:
-   'offer_variant' (A, B, C)
-   'cinverted' (0/1)
-   'click' / 'impressions'
-   'device', 'country' or other segements
-   Encode categorical variables where needed

### 4. Descriptive Statistics & EDA
- Compute summary statistics by offer:
    - Conversion rate
    - Click-through rate (CTR)
    - Average time on page/sessions
- Visualize distributions with:
    - Bar charts (conversion by offer)
    - Boxplots/histograms (time on page, sessions)
- Segment users by device, channel, or country to understand behavior

### 5. Hypothesis Testing
- **Two group comparisons (if needed):**
  - Use a proportion z-test or t-test to compare two offers/
- **Multi-group comparison:**
  - Use **ANOVA** to test if there are statistically significant differences in:
    - Conversion rate across all offers
    - Average time on page/engagement metrics
- Check assumptions (normality, variance) where appropriate.

### 6. Effect Size & Confidence Intervals
- Calculate confidence intervals for:
  - Conversion rate of each offer.
- Compute effect sizes (e.g., Cohen’s d or difference in proportions) to measure the practical impact of the winning offer.

### 7. Additional Analyses (Optional but Strong)
- Run segmented tests:
  - By device (mobile vs desktop)
  - By country or traffic source
- Explore interaction effects:
  - *Does a certain offer work better on mobile users than desktop users?*

### 8. Business Interpretation & Recommendations
- Translate statistical results into business language:
  - Identify the winning subscription offer.
  - Quantify expected lift in conversion and/or revenue.
- Discuss trade-offs (e.g., discount vs margin).
- Provide recommendations for rollout or follow-up experiments.

### 9. Project Structure & Reproducibility
- Organize the repository with:
  - `data/` – raw or sample data (or link to Kaggle)
  - `notebooks/` – Jupyter notebooks for EDA and analysis
  - `scripts/` – reusable Python scripts (if applicable)
  - `reports/` – exported plots or summary report
- Include instructions on how to run the notebook and reproduce results.

---
## Key Outcomes

- Identify the best-performing subscription offer based on statistical evidence.  
- Demonstrate skills in descriptive statistics, A/B testing, hypothesis testing, and ANOVA.  
- Provide clear, actionable recommendations for marketing and product teams.
