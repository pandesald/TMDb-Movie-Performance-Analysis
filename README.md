# TMDb Movie Performance Analysis
### EDA Case Study | Silver Screen Studios (Fictional)

## Dataset
Full TMDB Movies Dataset 2024 — available on
[Kaggle](https://www.kaggle.com/datasets/asaniczka/tmdb-movies-dataset-2023-930k-movies).

## Overview
Exploratory data analysis of 1.4M+ movie records from The Movie Database (TMDb), structured as a business case study for Silver Screen Studios — a fictional film production company seeking to improve its investment strategy.

## Objectives
- Analyze historical trends and patterns in movie production across years, decades, and release periods.
- Evaluate movie financial performance through budget, revenue, profit, ROI, and their relationships.
- Examine audience reception and genre performance using ratings, vote counts, runtime, production volume, and financial outcomes.
- Communicate key findings through clear visualizations, analytical observations, and business-oriented storytelling.

## Key Findings
- Only 58% of films with complete financial records were profitable — roughly 42 in 100 failed to recoup production costs.
- Budget and revenue are moderately correlated (r = 0.59), but budget alone does not determine commercial outcomes.
- December and July produce the highest median box-office revenues.
- Adventure and Animation lead on revenue; Documentary and Music lead on audience ratings.

## Business Implications
1. **Prioritize December and July release windows for major productions.** Both months consistently deliver the highest median box-office revenue in the dataset, with $8.2M and $7.5M respectively. For Silver Screen Studios, scheduling high-budget productions around these windows reduces the timing-related revenue risk.
2. **Treat production budget as necessary but not sufficient.** The moderate correlation between budget and revenue (r = 0.590) confirms that investment level matters. However, the wide dispersion in outcomes means that increasing the budget does not guarantee proportional financial returns. Genre selection, release timing, and creative execution each contribute independently.
3. **Align genre selection to project goals.** Adventure and Family genres carry the strongest historical revenue track records. Documentary and Music genres carry the strongest audience rating track records. Silver Screen Studios should define its primary success criterion per project such as financial return, critical reception, or both before committing to a genre, since optimizing for one does not reliably produce the other.
4. **Apply a realistic profitability benchmark to every greenlight decision.** With only 58% of financially-reported films achieving profitability, Silver Screen Studios should treat commercial success as probable rather than certain and build project approval frameworks that explicitly account for the realistic likelihood of loss before production begins.

## Limitations
- **Financial data coverage** - Budget and revenue records are only available for a small fraction of the full dataset. Findings reflect films large enough to have reported box-office figures, which biases results toward major studio productions. Smaller and independent films are underrepresented.
- **No inflation adjustment** - Revenue and budget figures are nominal values. Comparing financial figures across decades overstates the revenue of recent films relative to older productions and should be interpreted with caution.
- **Platform-specific ratings** - Audience ratings reflect TMDb users, a self-selected online audience. They may not represent the general moviegoing public or critical consensus.
- **Correlation does not imply causation** - Relationships identified in this analysis describe historical associations within the dataset and do not establish causal mechanisms.
- **Metadata completeness** - The dataset may contain incomplete, synthetic, or inconsistent metadata that affects certain analyses, particularly for older or less prominent productions.
- **Subset scope** - Financial analyses are restricted to released films with both budget and revenue reported. Audience analyses are restricted to released films with at least 10 votes. Findings do not generalize to the full 1.4M-record dataset.

## Conclusion

This exploratory analysis examined historical movie data from the TMDb dataset to address the core business problem facing Silver Screen Studios: understanding which factors are most consistently associated with commercial and critical success in film production.

The findings show that production budget carries a moderate positive relationship with box-office revenue, but the wide variation in financial outcomes across films with similar budgets confirms that investment level alone cannot guarantee returns. Release timing and genre both show meaningful differences in typical performance, December and July emerge as the strongest revenue windows, while Adventure and Animation lead commercially. The profitability analysis reveals that roughly 42 in 100 films with reported financial data failed to recover their production costs, establishing a baseline risk rate that Silver Screen Studios should incorporate into its project evaluation process.

For Silver Screen Studios, the most actionable output of this analysis is a clearer evidential foundation for investment decisions: which release windows carry a revenue advantage, which genres align with financial versus critical objectives, and what the realistic probability of commercial failure looks like at the industry level. These findings do not predict the outcome of any individual film, but they provide the historical context that separates data-informed decisions from intuition-based ones. Further work, such as revenue prediction modeling and franchise versus original IP analysis would extend these findings into more precise decision-support tools for the studio's investment committee.

## Tools & Libraries
Python · Pandas · NumPy · Matplotlib · Seaborn · Jupyter Notebook
