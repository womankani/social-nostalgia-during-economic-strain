# Social Nostalgia During Economic Strain
An empirical study of how economic pressure influences social trends that are driven by nostalgia in fashion, cinema, and technology.

## Motivation
Economic instability is often accompanied by the return of certain previously prominent social trends. This is most notably  observed in the revival of vintage-style clothing, increased appeal of cinematic reboots, and an uptick in the sales of retro technologies. Such patterns imply that when ground reality feels unstable, people look to the past for comfort.

This project investigates whether the effects of economic strain on the resurgence of social trends with nostalgic value are reflected in empirical data.

**Research Question:**
What is the impact of economic stress on the revival of older societal trends in fashion, cinema, and technology?

## Data
### Social Trends
- Mentions and popularity scores for past notable trends in:
  - Fashion (e.g. bell-bottoms, large collars)
  - Cinema (e.g. reboots, remakes)
  - Technology (retro technologies, vintage devices)
- Sources include internet archives, Vogue archives, IMDb,and Google Trends
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
Mentions and popularity scores of individual trends across categories are standardized (z-scored) to facilitate comparison of indicators from different sources and time periods. These scores are then combined to create categorical indices (fashion, cinema, technology). Categorical indices make up a composite Trend Popularity Index, which represents societal engagement with formerly prominent trends.

### Calculating Economic Strain
Economic pressure is represented by an economic stress index constructed through the standardization (z-scoring) and aggregation of unemployment rate, inflation rate and income growth, the last of which is inverted. This accounts for multiple factors contributing to economic pressure without placing disproportionate value on one variable.

A binary stress indicator is also constructed to mark periods of extreme economic strain. It is based off the stress index, where a stress value of above 0 coincides with 1 on the binary scale, and a value of below 0 coincides with 0.

### Timing and Lag Structure
Economic stress is unlikely to trigger an immediate social response. It is more probable that the stimulus of immense stress will cause an initial disturbance in the consumption, but will then lead to an increase in engagement with trends. To account for this, the analysis examines social popularity indices both concurrently and with time lags.

Lagging the social indices aligns future social responses with past economic data, allowing for the distinction between initial disruption and later trend revival as a behavioral consequence of economic stress.

## Key Visualizations & What They Show
<img width="560" height="356" alt="Economic Stress Index vs  Trend Popularity Index over Time" src="https://github.com/user-attachments/assets/2794d49a-46bb-4618-9e1c-5c0da7d90645" />

Fig. 1 shows effects of economic stress on social trends are not instantaneous

<img width="600" height="371" alt="Trend Popularity Index overlaid with High Stress Shading over Time" src="https://github.com/user-attachments/assets/981c2d58-4918-4b67-8036-cffa3c17b055" />

Fig 2. shows pattern followed by and behaviour of Trend Popularity Index during periods of high stress

<img width="649" height="401" alt="Average Trend Popularity in Low Stress   High Stress Years" src="https://github.com/user-attachments/assets/936d3d9f-9dec-467b-af0d-8d4b6e1b07e6" />

Fig 3. shows average trend popularity in years with high and low stress, suggesting engagement with trends declines in high stress years and supporting the theory of economic stress initially disrupting social behaviour

<img width="537" height="332" alt="Average Trend Popularity (Lag-2) in High Stress   Low Stress Years " src="https://github.com/user-attachments/assets/9a7dd842-2106-4b3e-8aae-94ef75f57700" />

Fig 4. shows average lagged trend populariy in high-stress and low-stress years, with a positive value for high-stress years. Supports theory that trends resurge following stimulus of economic stress.

<img width="518" height="321" alt="Trend Popularity Around Stress Year" src="https://github.com/user-attachments/assets/c55e7f32-4e3e-440e-8697-e4d8a0a5c484" />

Fig 5. shows trend popularity over years before, during and after high stress year, marking pattern of engagement with trends over five years for each stress episode

<img width="637" height="394" alt="Trend Popularity by Sector vs  Economic Stress over Time" src="https://github.com/user-attachments/assets/c07bf893-6ca1-415e-94aa-e08a87eab5af" />

Fig 6. shows the relative uniformity of categorical indices that make up the Trend Popularity Index alongside economic stress

## Key Findings
1. **Same-year relationships are weak.**
Concurrent comparisons show weak or unclear relationships between economic stress and increased trend popularity within the same year. OLS run on same year relationships returned a negative coefficient, further supporting the finding.
2. **Consumption and trend popularity goes down during stress.**
Average trend popularity is lower during high-stress years, suggesting that an influx of economic pressure disrupts social trends and consumption rather than immediately triggering trend resurgence.
3. **Nostalgia-seeking behaviour emerges later, as trends surge again.**
Event-style graphs and lagged comparisons demonstrate trend resurgence in the years following magnified economic strain. OLS run on lagged relationships returned a small positive coefficient, supporting the finding.
4. **The pattern is consistent across categories.**
Categorical breakup of the trend popularity index into sectors like fashion, cinema and technology demonstrates similar delayed trend resurgence, indicating a broad social reaction instead of a category-specific phenomenon.

These findings emphasize on the importance of timing when noting a social reaction to an economic stimulus. The nostalgia-driven resurgence of certain trends appears to be not an immediate reaction to economic strain, but rather a delayed response that materializes as stress persists.

## Interpretation
The results of the study suggest that past a certain threshold, economic stress initially suppresses social activity related to engaging with popular trends. This is likely reflective of typical nerves when facing financial instability. However, as conditions persist or even begin to ease, the rising popularity of significant trends is a distinct indicator of individual gravitation towards familiar icons, like combat-style boots or typewriters. This behaviour may be a coping mechanism that manifests as approaching nostalgia in an attempt to seek comfort in times of economic strain.

## Limitations
- Social nostalgia and trend popularity is measured indirectly through archives and online mentions.
- Annual frequency of the data limits ability to identify short-term dynamics and relationships.
- Analysis is observational and not does not establish causal mechanisms or predictive patterns.

## Repository Structure
trend-resurgence-project/
├── data/
│   ├── indices
│   ├── raw data
├── notebooks/
├── outputs/
│   ├── figures
└── README.md

## Future Work
- Sourcing trend popularity data through more direct sources for increased reliability.
- Increasing the frequency of data to gain short-term insights.
- Utilizing machine learning to assess predictive patterns.
  
## Summary
Prompted by the observation that people tend to re-engage with familiar forms of social activity, such as rewatching previously released films, this project shows that economic stress affects social behaviour in different ways. At first, the effect produced is of disruption when engagement with trends goes down, revealing a behavioural shift towards caution and conservation. Later, over time with stress persisting, trends across the categories of fashion, cinema and technology surge. This resurgence is an indicator that the comeback of trends reveals the societal affinity to use nostalgia as a coping mechanism during periods of economic instablity. 
