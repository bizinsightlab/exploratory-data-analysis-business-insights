# Chicago Taxi Market Exploration & Weather Impact Analysis

## Objective
This project combined exploratory data analysis in Python with structured SQL database queries to understand taxi ride dynamics in Chicago. The corporate goal was to map market share concentration among rival taxi companies, identify top drop-off destination hotspots, and statistically test whether weather conditions significantly impact average trip durations.

## Key Results
The analysis showed that Loop, River North, and Streeterville account for the vast majority of urban drop-offs in the city. By applying a Student's t-test, the null hypothesis was rejected, proving that average trip durations on Saturdays increase significantly under rainy weather conditions compared to clear days. This statistical insight supports the business case for dynamic pricing or extra driver incentives during severe weather.

## Tools & Technologies Used
- **Python** (Pandas, Matplotlib, Seaborn)
- **SciPy** (Inferential Statistical Analysis)
- **SQL** (Data extraction, joining weather logs with trip counts)

## What I Learned
- Consolidating and parsing data resulting from complex SQL queries containing aggregated and transactional logs.
- Crafting clear distribution and frequency visualizations (bar charts ranked by business relevance).
- Applying independent two-sample t-tests to validate operational logistics assumptions under external friction (weather metrics).

## Future Improvements
- Build a multiplier model to calculate the optimal surge pricing factor based on precipitation intensity.
- Expand the exploratory analysis to map rush-hour congestion patterns during regular weekdays.

---

## Methodology
1. **Competitor Analysis:** Imported and triaged ride volumes for various taxi companies operating in Chicago.
2. **Geographical Study:** Filtered and ranked the top 10 neighborhoods by average drop-off volume.
3. **Hypothesis Validation:** Segmented rides on specific Saturdays (clear vs. rainy) and applied Welch's t-test (`equal_var=False`).

## How to Run
1. Clone this repository.
2. Install the required dependencies: `pip install pandas scipy matplotlib seaborn`
3. Execute the notebook to review the urban logistics findings and statistical proofs.
