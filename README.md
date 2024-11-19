# Traveltime to Healthcare in the Democratic Republic of the Congo

# Healthcare Accessibility for Infants in the DRC

This project analyzes healthcare accessibility for infants aged 0-1 in the Democratic Republic of the Congo, focusing on those living more than 30 and 45 minutes driving distance from the nearest health facility. The analysis combines spatial datasets on population, travel time, and healthcare facility locations to produce visualizations and tables highlighting regions with limited healthcare access.

## Table of Contents
1. [Introduction](#introduction)
2. [Data Sources](#data-sources)
3. [Methods](#methods)
4. [Results](#results)
5. [How to Use](#how-to-use)
6. [Acknowledgments](#acknowledgments)

---

## Introduction

Access to healthcare is a critical issue in many developing countries, especially for vulnerable populations such as infants. This project visualizes and quantifies the number of infants aged 0-1 in the Democratic Republic of the Congo who face limited access to healthcare facilities, defined as living more than 30 or 45 minutes driving distance away. The project aims to provide actionable insights for planning healthcare interventions.

---

## Data Sources

1. **Population Data**:
   - WorldPop infant population datasets for ages 0-1 (male and female).
2. **Travel Time Data**:
   - Global motorized travel time dataset from Weiss et al. (2019).
3. **Healthcare Facility Locations**:
   - Healthsites.io database.
4. **Administrative Boundaries**:
   - GADM administrative boundaries (level 1 and 2).

---

## Methods

1. **Data Preprocessing**:
   - Clipped population and travel time rasters to the Democratic Republic of the Congo boundary.
   - Combined male and female infant population rasters to calculate the total infant population.

2. **Accessibility Analysis**:
   - Used the travel time raster to filter areas where infants live more than 30 or 45 minutes away from healthcare facilities.
   - Aggregated results by administrative boundaries using zonal statistics.

3. **Mapping and Visualization**:
   - Created a map showing the distribution of infants with limited healthcare access.
   - Highlighted healthcare facility locations and administrative boundaries for context.

4. **Summary Table**:
   - Generated a table showing the number of infants living more than 30 and 45 minutes away from healthcare facilities for each territory.

---

## Results

### Map
The map illustrates areas where infants aged 0-1 live more than 30 minutes driving distance from healthcare facilities. It also includes health facility locations and administrative boundaries.

### Summary Table
A table is provided that lists the number of infants in each territory who live more than 30 and 45 minutes driving distance from healthcare facilities.

---

## How to Use

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/infant-healthcare-access.git
   cd infant-healthcare-access
