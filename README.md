# Instagram & Meta Ads Performance Analysis

**Business Wisdom Institute (BWI)** runs organic Instagram content to build an audience and paid Meta ad campaigns to convert it into seminar leads. This project cleans and analyses **636 Instagram posts (May 2022 – Feb 2025)** and **13 Meta ad campaigns** to answer two questions:

1. Which organic content actually earns engagement, once audience size is accounted for?
2. Does the organic content history support or complicate what BWI's paid-ads reports concluded about creative performance?

![Engagement rate dashboard](BWI%2022-25%20PBI%20engagement%20rate.png)

## Key findings

- **Documentation posts earn the highest engagement rate (6.56%)**, while **Promotional posts, the most frequently published category (128 posts), earn the lowest (4.19%)**. The type BWI posts most is the one its audience engages with least.
- [Finding from your regression, e.g. which factor significantly predicts engagement]
- [Finding from the Meta Ads analysis, e.g. which creative had the highest CTR]

## Recommendations

- [Recommendation 1, e.g. shift part of the promotional volume towards documentation-style content]
- [Recommendation 2]

![Meta Ads CTR](BWI%2022-25%20Meta%20Ads%20CTR.png)

## Data cleaning

The raw export needed significant work before analysis:

- **~30 inconsistent content labels → 11 clean categories.** Merged abbreviations (BI / IB / Business Insight), mixed English and Indonesian labels, casing variants and multi-tagged posts.
- **107 missing posts recovered.** An initial weekday-based filter silently dropped May–Nov 2022; filtering on date validity restored the full 636-post history.
- **Impossible values handled.** One post recorded more likes than reach (a logging error); its engagement rate was excluded rather than guessed.
- Rebuilt a 3-row merged Excel header and fixed malformed dates and day values.

## Files

| File | Contents |
| --- | --- |
| [Analysis notebook](BWI%20Instagram%20Ads%20Analysis%2022-25.ipynb) | Python cleaning, analysis and regression |
| [Full report (PDF)](BWI_Instagram_Ads_Report_2022-2025.pdf) | Findings and recommendations for the marketing team |
| [Power BI dashboard (.pbix)](BWI%20Instagram%20Performance%20Report%2022-25.pbix) | Interactive dashboard (requires Power BI Desktop) |

## Tools

Python (pandas, matplotlib, statsmodels) · Power BI · Google Colab

*Raw data is not included for confidentiality.*
