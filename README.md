# BusinessAnalysis

## [Feature Engineering - Compare features for 2 Models](https://github.com/ChetanaYogeesh/BusinessAnalysis/blob/main/V2%20vs%20V1%20Performance%20Analysis%20-%20Executive%20Report.pdf)

<img width="899" height="806" alt="Screenshot 2026-01-20 at 8 34 54 PM" src="https://github.com/user-attachments/assets/8864ac61-3aac-4082-9925-02180af7a6dd" />

<img width="875" height="734" alt="Screenshot 2026-01-20 at 8 35 01 PM" src="https://github.com/user-attachments/assets/e3027a63-1b91-4b97-8ed6-4668a3796c15" />

<img width="869" height="723" alt="Screenshot 2026-01-20 at 8 35 08 PM" src="https://github.com/user-attachments/assets/a7adce3f-6d0e-44e2-8ebd-1edc3a93b8d8" />

<img width="860" height="410" alt="Screenshot 2026-01-20 at 8 36 40 PM" src="https://github.com/user-attachments/assets/c5926dd1-6cce-45fd-a220-08a155fb35e6" />

<img width="861" height="626" alt="Screenshot 2026-01-20 at 8 36 49 PM" src="https://github.com/user-attachments/assets/e9a32665-d3a6-4620-9fef-9ae4dd88d3de" />

## What We Know (Performance Differences)

### V2 performs WORSE than V1 across almost all metrics:

- **67% of products** show revenue decline in V2
- **$1,328 total revenue loss** in V2
- **3,274 fewer sales units** in V2
- **448 fewer add-to-cart actions** in V2
- **Worse search rankings** (average +10 positions lower in V2)

## What V1 and V2 Could Be

Based on the metrics being tracked and the patterns we see, V1 and V2 are likely comparing:

### Most Likely Scenarios

#### 1. Search/Recommendation Algorithm Versions
- **V1** = Old search/ranking algorithm
- **V2** = New search/ranking algorithm
- **Evidence**: Click position changes, search intent buckets, product ranking metrics

#### 2. E-commerce Platform Versions
- **V1** = Previous website/app version
- **V2** = New website/app version
- **Evidence**: Add-to-cart rates, online/offline sales tracking, UX metrics

#### 3. Pricing/Promotion Strategy Versions
- **V1** = Previous pricing model
- **V2** = New pricing model
- **Evidence**: Average unit price changes, margin % tracking

#### 4. Product Attribution Model Versions
- **V1** = Old method of attributing sales to segments
- **V2** = New attribution method
- **Evidence**: "attributed_to_segment" metrics throughout

## Evidence Points to Search/Recommendation System

The strongest evidence suggests V1 vs V2 is comparing **search or recommendation algorithm versions** because:

- Product click positions degraded significantly (+10 average, some +76 positions)
- Search intent buckets are tracked (Specific/Broad/Medium)
- Add-to-cart conversion rates changed
- "Specific" intent queries underperform vs "Broad" in V2

## What Likely Changed in V2

Based on the failure patterns:

1. **Search ranking algorithm changed** → Products appearing lower in results
2. **Product discovery logic changed** → Harder for customers to find products
3. **Offline channel integration issues** → 76% of decline from offline
4. **Regional rollout inconsistencies** → Region A failed, Region D succeeded

## To Determine Exactly What V1 and V2 Are

You would need to check:

- Project documentation or release notes
- What was deployed/changed between the measurement periods
- Whether this was an A/B test of algorithms, a platform upgrade, or a business rule change
- System change logs from the measurement period

---

## Chart Visualizations

### Overview Tab
- Stacked bar chart showing positive/negative/no change across all metrics
- Key metrics cards (67% declining, -$1,327 revenue, -3,274 units)
- Pie chart showing revenue impact distribution

### Products Tab
- Bar charts for top 5 products by revenue and sales impact
- Detailed table with all product metrics
- Shows Butter Product as biggest decline at -$713

### Segments Tab
- Performance comparison across Premium/Standard/Budget
- Win rate visualization
- Individual segment cards with detailed metrics
- Shows Premium segment as worst performer (-75% negative rate)

### Regions Tab
- Regional performance comparison
- Winning vs losing products by region
- Color-coded cards (green for positive, red for negative)
- Shows Region D as only winner, Region A as worst performer

### Impact Tab
- Overall business impact pie chart
- Channel analysis showing 76% offline decline
- Four key metric cards for quick reference
- Critical findings highlighted
