# rain-probability-analyzer
Historical Rain Probability Analyzer

Analytical tool developed in Python and Jupyter Notebook to evaluate historical climate data and support intelligent decision-making for outdoor events.

The project receives two inputs from the user, location and data, then queries open-source historical weather data, processes it into structured data, generates interactive visualizations, and leverages Large Language Models (LLMs) to output an interpretive risk summary.

### Methodology (Why the ±7 Days Window?)
Weather patterns can easily shift by a few days from year to year. If a severe cold front caused major downpours on May 24th in 2021 and May 28th in 2023, a strict lookup on May 26th would mathematically ignore these events, causing a false sense of security.

By evaluating a 15-day window (7 days prior and 7 days after the targeted date), this algorithm yields a robust, smoothed probability baseline representing the true macro-climate of that season.

### Technologies & Libraries

- **Language:** Python 3.11+
- **Environment:** Jupyter Notebook
- **Data Manipulation:** [Pandas](https://pandas.pydata.org/)
- **Visualizations:** [Plotly Express & Graph Objects](https://plotly.com/python/)
- **AI Integration:** Maritaca AI
