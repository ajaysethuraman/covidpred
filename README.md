
This script analyzes and visualizes COVID-19 cases in India using libraries like Pandas, Matplotlib, Seaborn, Plotly, Folium, and Prophet. Here's a concise breakdown of its components:

1. Data Import and Preprocessing
- Data Loading: Four datasets (Indian COVID cases, coordinates of states/UTs, and daily cases in India, Korea, Italy, Wuhan) are imported using pd.read_excel.
- Data Manipulation:
  - Dropped unnecessary columns.
  - Created new columns:
    - Total cases as the sum of Indian and foreign nationals.
    - Total Active by subtracting deaths and recoveries from total cases.

2. Basic Insights
- Summarized total and active cases.
- Highlighted data tables with color gradients using pandas.style.

3. Geospatial Analysis
- Merged COVID data with Indian state coordinates.
- Created an interactive map using Folium, where:
- Each state/UT is represented by a circle sized by its total cases.
- Popup displays state name and case details.

4. Visualization
- Bar Plots:
  - Compared total cases vs recovered using Seaborn.
- Line Charts:
  - Trends of cumulative cases over time via Plotly.
- Daily Case Reports:
  - Daily new cases visualized as bar charts using Plotly Express.

5. Forecasting with Prophet
- Used Facebook Prophet to predict:
  - Future confirmed cases.
  - Future deaths.
- Results include:
  - Forecast data with upper and lower bounds.
  - Plots for predictions and their components.

This script combines geospatial analysis, interactive visualizations, and machine learning forecasting to provide a comprehensive understanding of COVID-19 trends in India.
