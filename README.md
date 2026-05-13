# Virginia Data Center Electricity Analysis

This repository contains data analysis and visualizations for a DATA C104 research project on electricity classification, data centers, and infrastructural governance in Northern Virginia.

The project examines how data center electricity demand becomes visible, or hidden, through public electricity categories such as commercial, industrial, residential, and all-sector electricity data. The analysis uses U.S. Energy Information Administration (EIA) retail electricity data to study Virginia electricity sales, average prices, customer classes, and sector-level trends from 2010 to 2024.

## Project Overview

Northern Virginia has become one of the largest data center regions in the world. While this growth is often explained through land availability, tax incentives, fiber infrastructure, and proximity to federal institutions, this project focuses on the electricity systems that make that growth possible.

The central question is how data center demand is categorized, priced, forecasted, and governed through utility classifications. Since public EIA data does not isolate data centers as their own category, this project uses commercial-sector electricity trends as a way to study where data center demand is likely embedded.

## Research Context

The analysis supports a broader paper titled:

**Classifying the Cloud: GS-5, Data Centers, and Infrastructural Governance in Northern Virginia**

The paper argues that Dominion Energy Virginia’s GS-5 large general service tariff should be understood as a classification system, not just a billing category. Drawing on scholarship about classification, infrastructure, and sociotechnical systems, the project studies how data center growth becomes administratively manageable while its public consequences can become harder to trace.

## Data Source

The main dataset comes from the U.S. Energy Information Administration:

- **Dataset:** EIA Form EIA-861 Annual Electric Power Industry Report
- **API endpoint:** EIA Electricity Retail Sales API
- **Years covered:** 2010–2024
- **Geographies used:** Virginia, Maryland, North Carolina, Pennsylvania, and the United States
- **Sectors used:** Residential, Commercial, Industrial, and All Sectors
- **Metrics used:** Electricity sales, average price, revenue, and customer counts

## Main Visualizations

The notebook generates several figures used to support the research paper:

### 1. Virginia Electricity Sales Growth by Sector

Shows how electricity sales changed across residential, commercial, industrial, and all-sector categories in Virginia. Each sector is indexed to 2010, making it easier to compare relative growth.

### 2. Commercial Load Relative to Industrial Load

Compares commercial and industrial electricity demand in Virginia over time using a commercial-to-industrial ratio.

### 3. Year-over-Year Electricity Change

Shows annual percentage changes in commercial and industrial electricity sales/load to identify periods of rapid growth.

### 4. Commercial Sales vs Average Price

Compares indexed commercial electricity sales and average commercial electricity prices to show whether sales growth moved alongside price growth.

### 5. Commercial Sales Growth Across States

Compares Virginia’s commercial electricity sales growth with other states and the United States.

### 6. Average Retail Electricity Prices by Customer Class

Compares residential, commercial, industrial, and all-sector average retail electricity prices in Virginia from 2010 to 2024. Residential and commercial classes are emphasized because they are most relevant to the ratepayer and classification discussion.

### 7. Summary Table

Provides a concise comparison of 2010 sales, 2024 sales, growth percentage, 2024 average price, and 2024 customers for major Virginia sectors.

## To Run 
You will need to obtain an EIA API key for free and place the Key in the EIA Api field

## Repository Structure

```text
.
├── notebook.ipynb          # Main Jupyter notebook with data collection and figures
├── README.md               # Project description
├── .env                    # Local API key file, not committed
├── requirements.txt        # Python dependencies, optional
└── figures/                # Exported figures, optional
