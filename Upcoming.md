# Research Plan: Industrial Nightlight, Waste Production, and Economic Activity

## Epic 1: Data Acquisition, Processing, and Correlation Analysis

### 1. Collect EPA Waste Data

- Gather annual EPA datasets for multiple years.
- Standardize formats, extract facility identifiers, geographic coordinates, and waste output metrics.
- Construct a unified multi-year panel for trend analysis.

### 2. Analyse Waste Production Trends

- Compute annual changes in hazardous and non-hazardous waste output.
- Compare trends across factories, regions, and industrial categories.
- Identify outliers and facilities with unusual production or reporting behavior.

### 3. Acquire Annual Nightlight Data

- Download satellite-based nightlight imagery for each year of interest.
- Ensure consistent resolution, masking procedures, and preprocessing steps.

### 4. Identify Industrial Land Using External APIs

- Use building-footprint or land-classification APIs/tools that provide polygonal industrial or factory-area blocks.
- Combine these with EPA geolocations to isolate industrial zones.
- Construct binary/weighted spatial masks representing factory areas.

### 5. Create Industrial Land Mask for Nightlights

- Apply the industrial-area mask to nightlight rasters.
- Remove or ignore non-industrial pixels.
- Produce an annual time series of industrial-only luminosity.

### 6. Analyse Nightlight Trends in Industrial Zones

- Extract per-facility and industry-wide nightlight indicators.
- Examine trends in brightness, expansion, contraction, or seasonal patterns.
- Compare year-over-year changes to industrial growth or slowdown.

### 7. Compute Waste–Nightlight Correlations

- For each facility: correlate annual waste output with annual mean luminosity.
- For the industry: evaluate aggregate correlation statistics.
- Assess significance, robustness, and potential lags.

### 8. Optional: Higher-Frequency Trend Analysis

- If available, analyse monthly or daily nightlight readings.
- Measure intra-year fluctuations and potential operational cycles.

---

## Epic 2: Academic Collaboration and Extended Economic Analysis

### 1. Engage with Professors and Research Collaborators

- Present initial findings and visualizations.
- Gather feedback on methodology, assumptions, and next steps.

### 2. Acquire Production and Profitability Data

- Obtain plant-level production volumes and profit estimates.
- Merge with EPA waste datasets and nightlight indicators.

### 3. Assess Correlations with Economic Variables

- Test whether waste alone correlates weakly with profits/production due to misreporting or variability.
- Evaluate whether nightlight correlates strongly with economic output.
- Examine joint correlations among nightlight, waste metrics, revenue, production, and facility characteristics.

### 4. Pre-Process, Validate, and Document the Dataset

- Clean, normalize, and harmonize time series.
- Conduct robustness checks: stationarity, seasonality, outlier detection, and causal-direction analysis.

### 5. Prepare for Publication

- Draft a formal research paper including: motivation, data sources, methodology, model assumptions, empirical results, and limitations.
- Generate reproducible code notebooks and appendices.
- Submit to relevant conferences or journals focusing on environmental economics, remote sensing, or industrial analytics.
