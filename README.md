# Social Nostalgia During Economic Strain
An empirical study of how economic pressure influences social trends that are driven by nostalgia in fashion, cinema, and technology.

## Motivation
Economic instability is often accompanied by the return of certain social trends that were prominent in the past. This is most famously noted in the revival of vintage-style clothing, the increased appeal of cinematic reboots, and an uptick in the sales of retro technologies. Such patterns imply that when the ground reality feels unstable, people look to the past for comfort.

This project investigates whether the pattern of the effects of economic strain on the resurgence of social trends driven by nostalgia is reflected in empirical data.

**Research Question:**
What is the impact of economic stress on the revival of older societal trends in fashion, cinema, and technology?

## Data
### Social Trends
- Mentions and popularity indicators for past notable trends in:
  - Fashion (e.g. bell-bottoms, large collars, trends across decades)
  - Cinema (e.g. reboots, remakes)
  - Technology (retro technologies, vintage devices)
- Sources include magazine archives, IMDb,and Google Trends
- Measures are standardized and combined into categorical and composite "social popularity" indices
- Annual frequency, with a time frame of 1965-2025

### Economic Strain
- Single composite economic stress indice comprising:
  - Unemployment rate
  - Inflation rate
  - Real income growth (inverted)
- Sources include World Bank and FRED
- Variables are standardized and combined into an economic stress index
- Binary stress indicator based off stress index

## Methodology
### Social Popularity Indices
Mentions and popularity indicators of individual trends are standardized (z-scored) to facilitate comparison of indicators from different sources and time periods. These scores are then combined to create categorical indices (fashion, cinema, technology) and construct a composite Trend Popularity Index.

### Calculating Economic Strain
Economic pressure is represented by an economic stress index constructed through the standardization (z-scoring) and aggregation of unemployment rate, inflation rate and income growth, the last of which is inverted. This accounts for multiple factors contributing to economic pressure without placing disproportionate value on one variable.

A binary stress indicator is also constructed to mark periods of extreme economic strain.

### Timing and Lag Structure
Economic stress is unlikely to trigger an immediate social response. The stimulus of immense stress creating an initial disturbance in consumption trends, subsequently followed by an amplification, is more plausible. To account for this, the analysis examines social popularity indices both concurrently and with time lags.

Lagging the social indices aligns future social responses with past economic data, allowing for the distinction between initial disruption and later trend revival as a behavioral consequence of economic stress.

## Key Visualizations & What They Show
<img width="560" height="356" alt="Economic Stress Index vs  Trend Popularity Index over Time" src="https://github.com/user-attachments/assets/2794d49a-46bb-4618-9e1c-5c0da7d90645" />

Shows effects of economic stress on social trends are not instantaneous

<img width="600" height="371" alt="Trend Popularity Index overlaid with High Stress Shading over Time" src="https://github.com/user-attachments/assets/981c2d58-4918-4b67-8036-cffa3c17b055" />

Shows trend popularity pattern in periods of high stress

<img width="649" height="401" alt="Average Trend Popularity in Low Stress   High Stress Years" src="https://github.com/user-attachments/assets/936d3d9f-9dec-467b-af0d-8d4b6e1b07e6" />

Shows negative relationship between economic stress year and trend resurgence

<img width="537" height="332" alt="Average Trend Popularity (Lag-2) in High Stress   Low Stress Years " src="https://github.com/user-attachments/assets/9a7dd842-2106-4b3e-8aae-94ef75f57700" />

Shows positive relationship between economic stress years and lagged trend popularity indicating trends resurge after effect of stress has been experienced

<img width="518" height="321" alt="Trend Popularity Around Stress Year" src="https://github.com/user-attachments/assets/c55e7f32-4e3e-440e-8697-e4d8a0a5c484" />

Shows trend popularity over years before, during and after high stress year

<img width="637" height="394" alt="Trend Popularity by Sector vs  Economic Stress over Time" src="https://github.com/user-attachments/assets/c07bf893-6ca1-415e-94aa-e08a87eab5af" />

Shows the relative uniformity of categorical indices that make up trend popularity index alongside economic stress

## Key Findings
1. **Same-year relationships are weak.**
Concurrent comparisons show weak or unclear relationships between economic stress and increased trend popularity within the same year.
2. **Consumption and trend popularity goes down during stress.**
Average trend popularity is lower during high-stress years, suggesting that an influx of economic pressure disrupts social trends and consumption rather than immediately triggering trend resurgence.
3. **Nostalgia-seeking behaviour emerges later, as trends surge again.**
Event-style graphs and lagged comparisons demonstrate trend resurgence in the years following magnified economic strain.
4. **The pattern is consistent across categories.**
Categorical breakup of the trend popularity index into sectors like fashion, cinema and technology demonstrates similar delayed trend resurgence, indicating a broad social reaction instead of a category-specific phenomenon.

These findings emphasize on the importance of timing when noting a social reaction to an economic stimulus. The nostalgia-driven resurgence of certain trends appears to be not an immediate reaction to economic strain, but rather a delayed response that materializes as stress persists.

## Interpretation
The results of the study suggest that initially and past a certain threshold, economic stress suppresses social trend-related activity. This likely reflects wariness and uncertainty. As conditions persist or ease, however, the rising popularity of significant trends indicates individual gravitation towards familiar and iconic objects. This behaviour may be driven by nostalgia in a comfort-seeking attempt to find some stability during uncertain times.

## Limitations
- Social nostalgia and trend popularity is measured indirectly through archives and online mentions.
- Annual frequency of the data limits ability to identify short-term dynamics and relationships.
- Analysis is observational and not does not establish causal mechanisms or predictive patterns.

## Repository Structure
trend-resurgence-project/
├── README.md
├── data/
├── notebooks/
├── outputs/
└── scripts/

## Future Work
- Sourcing trend popularity data through more direct sources for increased reliability.
- Increasing the frequency of data to gain short-term insights.
- Utilizing machine learning to assess predictive patterns.
  
## Summary
Prompted by the observation that people tend to return to familiar social forms during harsh times, this project shows that economic stress affects social behaviour in different ways. Originally the effect produced is social disruption when consumption of trends goes down, revealing a shift towards uncertainty and fear. Later, over time with the stress persisting, past trends resurge on a delayed basis, indicating that social trend resurgence behaves as a coping mechanism during periods of instability.
