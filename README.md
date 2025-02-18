# Financial Performance Dashboard (Power BI)

This Power BI dashboard provides a comprehensive overview of financial performance, enabling data-driven decision-making through interactive visualizations and key performance indicators (KPIs).

## Project Overview

This project aimed to create a dynamic and informative dashboard to track and analyze financial performance.
Data from an Excel spreadsheet was loaded into Power BI, transformed and cleaned, and then used to create interactive visualizations and calculated measures. 
This dashboard empowers users to monitor key metrics, identify trends, and make informed strategic decisions.

## Data Source

The data for this dashboard originates from an Excel spreadsheet.

## Data Transformation and EDA

The following steps were performed to prepare and analyze the data:

1.  **Data Loading:** The data from the Excel spreadsheet was loaded into Power BI.

2.  **Data Transformation:**  Extensive data cleaning and preprocessing was performed, including:
    *   Handling null and missing values using appropriate techniques (e.g., imputation or removal). *(Mention specific methods if used)*
    *   Updating data types to ensure compatibility with calculations and visualizations (e.g., converting date fields, ensuring numerical fields are formatted correctly).  *(Mention specific examples if applicable)*
    *   *(Optional: Mention any other transformations performed, such as creating calculated columns or merging data from multiple sources.)*

3.  **Exploratory Data Analysis (EDA):**  EDA was conducted to understand the data's characteristics, identify patterns, and inform the creation of meaningful visualizations.

## Measures Created

The following key measures were created in Power BI using DAX (Data Analysis Expressions):

*   `Total Sales`: The sum of all sales amounts('Total Sales Actual = SUM(Actual[Sales])').
*   `Total Sales Target`: The sum of all sales target amounts ('Total Sales Target = SUM(Targets[Sales])').
*   `Variance`: The difference between Total Sales and Total Sales Target (`Variance = [Total Sales Actual]-[Total Sales Target]`).
*   `Variance %`: The percentage variance from the sales target `Variance % = DIVIDE([Variance],[Total Sales Actual])`.
*   `YTD Sales Actual`: Year-to-date sales actual('YTD Sales Actual = CALCULATE([Total Sales Actual],DATESYTD('Calendar'[Date]))').
*   `YTD Sales Target`: Year-to-date sales target.
*   `YTD Variance`: Year-to-date variance (`YTD Variance = CALCULATE([Variance],DATESYTD('Calendar'[Date]))`).
*   `YTD Variance %`: Year-to-date percentage variance `(YTD Variance % = CALCULATE([Variance %],DATESYTD('Calendar'[Date]))`.

## Interactive Visualizations

The dashboard features interactive visualizations to facilitate data exploration and analysis, including:

*   *   Stacked Bar Chart to Visualize Total Sales Actual vs Total Sales Target.
    *   KPI cards displaying key metrics.
    *   Description regarding the Trend and Data.
    *   Filters based on Teams.
    *   Line chart to display trends for each sales person

## Key Features

*   **Interactive Exploration:** Users can interact with the visualizations and filters to explore the data and drill down into specific details.
*   **Key Performance Indicators (KPIs):** The dashboard prominently displays key financial metrics, providing a quick overview of performance.
*   **Trend Analysis:** Visualizations enable users to identify trends and patterns in the data over time.
*   **Data-Driven Decisions:** The dashboard provides actionable insights to support informed decision-making.
