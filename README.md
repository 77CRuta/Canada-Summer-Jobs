# Canada Summer Jobs (CSJ) 2024 — Findings Summary

## Dataset Overview

| Metric | Value |
|--------|-------|
| **Total Constituencies** | 338 |
| **Total Amount Paid** | $293,372,944 |
| **Total Jobs Created** | 71,204 |
| **National Avg Cost Per Job** | $4,120.18 |

---

## Distribution of Cost Per Job

The histogram below shows how cost per job is distributed across all 338 constituencies. The curve overlay (KDE) shows the overall density shape.

![Distribution of Cost Per Job](plots/distribution_histogram.png)

---

## Top 10 Most & Least Expensive Constituencies

The side-by-side comparison below highlights the **least cost-efficient** (left, red) and **most cost-efficient** (right, green) constituencies by cost per job.

![Top 10 vs Bottom 10 Cost Per Job](plots/top_bottom_10.png)

### Least Cost-Efficient (Highest Cost Per Job)

| Rank | Constituency | Amount Paid | Jobs Created | Cost Per Job |
|------|-------------|-------------|--------------|-------------|
| 1 | Oakville-Nord - Burlington | $1,076,698 | 162 | **$6,646.28** |
| 2 | Notre-Dame-de-Grâce - Westmount | $1,108,905 | 183 | **$6,060.14** |
| 3 | LaSalle - Émard - Verdun | $1,105,106 | 183 | **$6,050.31** |
| 4 | Ville-Marie - Le Sud-Ouest - Île-des-Soeurs | $1,102,250 | 183 | **$6,023.12** |
| 5 | Vancouver Kingsway | $712,915 | 120 | **$5,941.96** |
| 6 | Vancouver-Centre | $666,249 | 115 | **$5,793.47** |
| 7 | Kitchener-Centre | $659,702 | 114 | **$5,787.74** |
| 8 | Fort Saskatchewan | $553,339 | 96 | **$5,763.95** |
| 9 | Outremont | $655,536 | 116 | **$5,651.17** |
| 10 | Toronto-Centre | $668,932 | 119 | **$5,621.28** |

### Most Cost-Efficient (Lowest Cost Per Job)

| Rank | Constituency | Amount Paid | Jobs Created | Cost Per Job |
|------|-------------|-------------|--------------|-------------|
| 1 | Lakeland | $489,677 | 169 | **$2,897.85** |
| 2 | Battle River - Crowfoot | $499,004 | 170 | **$2,935.32** |
| 3 | Yorkton - Melville | $494,422 | 167 | **$2,960.61** |
| 4 | Cypress Hills - Grasslands | $482,417 | 163 | **$2,960.23** |
| 5 | Moose Jaw - Lake Centre - Lanigan | $509,552 | 167 | **$3,051.21** |
| 6 | Prince Albert | $554,765 | 183 | **$3,032.05** |
| 7 | Lethbridge | $510,426 | 168 | **$3,038.25** |
| 8 | Desnethé - Missinippi - Rivière Churchill | $508,178 | 167 | **$3,043.60** |
| 9 | Carleton | $740,873 | 241 | **$3,074.16** |
| 10 | Malpeque | $529,391 | 170 | **$3,114.06** |

---

## Edmonton vs Calgary Comparison

A direct comparison of the two largest Alberta cities across total funding, jobs created, and cost efficiency.

![Edmonton vs Calgary Comparison](plots/edmonton_vs_calgary.png)

### Edmonton

| Metric | Value |
|--------|-------|
| **Constituencies** | 9 |
| **Total Paid** | $8,804,926 |
| **Total Jobs** | 2,239 |
| **Avg Cost Per Job** | $3,932.53 |
| **Min / Max CPJ** | $3,225 — $4,759 |

### Calgary

| Metric | Value |
|--------|-------|
| **Constituencies** | 10 |
| **Total Paid** | $10,309,459 |
| **Total Jobs** | 2,711 |
| **Avg Cost Per Job** | $3,802.83 |
| **Min / Max CPJ** | $3,283 — $4,915 |

> 📊 **Takeaway:** Calgary spent more overall ($10.3M vs $8.8M) and created more jobs (2,711 vs 2,239), but at a **lower cost per job** ($3,803 vs $3,933) — about $130 cheaper per job.

---

## City Scatterplot — Calgary vs Vancouver vs Edmonton

Each dot represents a single constituency. The vertical position shows its cost per job, making it easy to spot patterns and outliers within each city.

![City Scatterplot](plots/city_scatterplot.png)

---

## City Comparison at a Glance

| City | Constituencies | Total Paid | Total Jobs | Cost Per Job |
|------|---------------|------------|------------|-------------|
| Calgary | 10 | $10,309,459 | 2,711 | **$3,802.83** 🟢 |
| Edmonton | 9 | $8,804,926 | 2,239 | **$3,932.53** |
| Toronto | 3 | $2,915,847 | 638 | **$4,570.29** |
| Vancouver | 8 | $5,979,087 | 1,130 | **$5,291.23** 🔴 |
| *National Avg* | *338* | *$293,372,944* | *71,204* | *$4,120.18* |

### Key Takeaways

1. **Calgary is the most cost-efficient** of the four cities — $3,803 per job, well below the national average
2. **Vancouver is the least cost-efficient** — $5,291 per job, 28% above the national average
3. **Edmonton and Calgary** both beat the national average, with Calgary edging ahead
4. **Toronto** falls in the middle, slightly above the national average
5. The **national spread** ranges from ~$2,898 to ~$6,646 — a **$3,748 gap** between most and least efficient

---

*Analysis based on Canada Summer Jobs 2024 results data (`csj-results-cleaned.csv`)*
