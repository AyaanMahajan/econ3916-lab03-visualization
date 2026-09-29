# Honest vs. Misleading Visualizations

## Objective
This project looks at how visualization choices can change the story a reader takes away from the same economic data, even when the underlying numbers do not change.

## Methodology
- Recreated Anscombe's Quartet and compared the plots with nearly identical summary statistics.
- Calculated a Lie Factor of 49.0 for a revenue chart with a truncated y-axis and compared it with an honest redesign.
- Deflated FRED average hourly earnings into 2020 dollars and plotted the same real wage series four different ways.
- Used a four-step EDA process on World Bank GDP data: structure, distributions, relationships, and anomalies.
- Compared raw GDP with log-transformed GDP to deal with extreme right skew.
- Built an interactive wage chart that switches between nominal and real earnings, changes the time window and axis scale, and shows how the y-axis floor changes the Lie Factor.

## Key Findings
- Anscombe's Quartet shows why summary statistics are not enough on their own. Data with very similar means, variances, correlations, and regression lines can have completely different shapes.
- The truncated revenue chart had a Lie Factor of 49.0, meaning the visual effect was about 49 times the actual percentage change.
- Real wages tell a much less dramatic long-run story than nominal wages because nominal wages include inflation.
- The World Bank GDP data covers 266 economies and regional aggregates across 64 years (1960–2023). GDP is extremely right-skewed, and a log transformation makes the distribution much easier to interpret.
- Missing GDP coverage is concentrated near the beginning and end of the period rather than being randomly scattered.
- Raising the y-axis floor can make a small change look much larger, which is why scale and baseline choices should always be checked before trusting a chart.
