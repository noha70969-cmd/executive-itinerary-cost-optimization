# Executive Itinerary Cost Optimization

**Excel Data Analysis Portfolio Project**

## 1. Project Overview

This project analyzes 200 synthetic business trip records covering January to June 2026 to identify major cost drivers and explore opportunities to optimize business trip costs without compromising business requirements or service quality.

Using Microsoft Excel 2021 and Power Query, the project demonstrates an end-to-end analytical workflow, including data cleaning, data preparation, analysis, PivotTables, and interactive dashboard development.

The objective is to identify spending patterns and evaluate business travel factors to support informed cost optimization decisions.

## 2. Business Problem

Business travel is an important operational activity, but it can represent a significant expense for organizations. Without a clear understanding of spending patterns, it can be difficult to identify where costs are concentrated and where optimization opportunities exist.

This project addresses the need to analyze business travel expenses, understand the factors influencing trip costs, and identify potential opportunities to reduce spending while maintaining business requirements and service quality.

## 3. Project Objectives

- Analyze business trip expenses to identify the main cost drivers.
- Compare travel costs across trip purposes, hotel categories, flight types, business priorities, and airlines.
- Identify spending patterns and potential cost-optimization opportunities.
- Develop an interactive Excel dashboard to support data exploration and decision-making.
- Provide practical recommendations while maintaining business requirements and service quality.

  ## 4. Dataset Description

The project uses a dataset of 200 synthetic business trip records covering the period from January to June 2026.

The original dataset contains 19 fields describing business trips, including:

- Trip dates and destinations
- Trip purpose and business priority
- Traveler type
- Flight details, airline, and travel costs
- Hotel category, number of nights, and accommodation costs
- Ground transport and other expenses

After data preparation, the cleaned dataset contains 24 fields, including additional calculated columns created to support the analysis.

## 5. Dataset Disclaimer

This project uses a synthetic dataset created for educational and portfolio demonstration purposes. The business trip records, expense figures, and prices are illustrative examples and do not represent actual company travel records, real transactions, or current market prices.

The dataset was designed to simulate a business travel environment and demonstrate data cleaning, analysis, cost evaluation, and dashboard development using Microsoft Excel and Power Query.

## 6. Data Cleaning & Preparation

Microsoft Excel Power Query was used to clean and prepare the dataset before analysis.

The preparation process included:

- Reviewing the original dataset structure and data fields.
- Identifying and removing a duplicate trip record (Trip T025).
- Reviewing missing and incomplete values.
- Applying appropriate data types and formatting.
- Creating a cleaned dataset for analysis.
- Loading the prepared data into Excel for PivotTable analysis and dashboard development.

The original dataset contained 201 records. After removing the duplicate record, the cleaned dataset contained 200 business trip records.

## 7. Calculated Fields & Their Purpose

Five additional fields were created during data preparation to support the analysis:

| Calculated Field | Purpose |
|---|---|
| Booking Lead Time | Measures the number of days between booking and departure to examine booking patterns. |
| Total Trip Cost | Calculates the combined cost of flights, hotels, ground transport, and other expenses. |
| Trip Duration | Measures the number of days between departure and return dates. |
| Hotel Cost per Night | Calculates the hotel cost per night to enable fair comparisons across hotel categories. |
| Priority Check | Uses text length to help identify potential inconsistencies in business priority labels. |

These fields support more detailed comparisons and help answer the project's analytical questions.

**Note:** Priority Check is a helper field based on text length. It can help identify potential inconsistencies in business priority labels, but it does not independently confirm that every label is correct.

## 8. Data Quality & Limitations

During data preparation and validation, the following data quality issues were identified:

| Trip ID | Data Quality Issue | Impact |
|---|---|---|
| T057 | Missing hotel cost. | Total Trip Cost is blank, so this record is excluded from calculations based on non blank Total Trip Cost values. |
| T143 | Missing ground transport cost. | The missing component is treated as zero in the calculated trip cost, which may understate the actual cost. |
| T168 | Other Expenses recorded as zero. | The original value could not be independently confirmed, so this record should be interpreted with caution. |
| T092 | Ambiguous booking date (02/03/2026). | The date format could not be confirmed, so no assumption was made about its intended date. |

**Validation Summary**

- Total dataset records: 200 trips.
- Records with non blank Total Trip Cost: 199.
- Total Known Expenses: SAR 1,045,507.09.
- Sum of Total Trip Cost: SAR 1,041,212.93.
- Difference between the two totals: SAR 4,294.16.

The two totals are reported separately because they are calculated using different approaches. The difference has not been fully reconciled and should not be interpreted as savings or cost reduction.

These limitations should be considered when interpreting the analysis and recommendations.

## 9. Analytical Approach

The project followed a structured analytical workflow:

1. **Understand the Business Problem:** Define the objective of optimizing business travel costs without compromising quality or business requirements.
2. **Prepare the Data:** Review, clean, and transform the original dataset using Power Query.
3. **Create Calculated Fields:** Add relevant fields to support cost calculations and comparisons.
4. **Analyze the Data:** Use Excel PivotTables to explore spending patterns and compare different business travel factors.
5. **Identify Insights:** Interpret the results to identify major cost drivers and potential optimization opportunities.
6. **Develop Recommendations:** Translate the findings into practical recommendations to support informed decisions.
7. **Build the Dashboard:** Present key findings through an interactive Excel dashboard with charts, slicers, and a timeline.
8. **Validate the Results:** Cross-check calculations and review data quality limitations to support reliable interpretation.

## 10. Analysis Selection & Rationale

The initial expense breakdown identified Flights and Hotels as the two largest expense components:

- Flights: SAR 499,927.96 (47.82%).
- Hotels: SAR 464,267.80 (44.41%).

Together, these two categories accounted for 92.23% of Total Known Expenses.

Based on this initial finding, five focused analyses were selected:

1. Trip Purpose Costs
2. Hotel Category Comparison
3. Flight Comparison
4. Trip Priority
5. Airline Comparison

These analyses were chosen to investigate the main cost drivers, understand spending patterns, and identify practical cost-optimization opportunities.

The analysis sequence reflects the project's findings and keeps the focus on insights that can support business decisions.

## 11. Key Findings

### 1. Trip Purpose Costs

Internal Meetings recorded the highest total trip cost at SAR 188,221.06, followed by Project Meetings at SAR 164,460.11.

### 2. Hotel Category Comparison

Category 5 hotels recorded the highest average cost per night at SAR 934.72, approximately 40.5% higher than Category 4 hotels.

### 3. Flight Comparison

Direct flights had a higher average cost of SAR 2,635.45 compared with SAR 2,150.43 for connecting flights. However, direct flights reduced average travel time from 7.78 hours to 4.12 hours.

### 4. Trip Priority

Medium-priority trips represented the largest group, with 107 trips, and recorded the highest average total trip cost at SAR 5,450.34.

### 5. Airline Comparison

Airline B recorded the highest average flight cost at SAR 2,787.06, while Airline D recorded the lowest at SAR 2,356.08.

**Note:** The dataset contains 200 business trip records; however, total trip cost analysis is based on 199 non blank records due to the missing hotel cost for Trip T057. This limitation is documented in the Data Quality & Limitations section.

## 12. Recommendations

Based on the analysis, the following recommendations are proposed:

1. **Trip Purpose:** Review spending associated with Internal Meetings and Project Meetings to identify opportunities to optimize travel arrangements while maintaining essential business activities.

2. **Hotel Category:** Evaluate the use of Category 5 hotels and consider Category 4 as a potential cost-saving alternative where accommodation quality and business requirements are met.

3. **Flight Selection:** Consider direct flights when time savings justify the additional cost. Connecting flights may be more suitable when budget savings are a priority and longer travel times are acceptable.

4. **Business Priority:** Review medium-priority trips to identify potential cost-optimization opportunities while maintaining business objectives and operational requirements.

5. **Airline Selection:** Evaluate airline options based on average flight costs, while also considering route availability, travel duration, and service requirements.

Overall, travel decisions should balance cost efficiency, time, service quality, and business needs rather than focusing on cost reduction alone.

## 13. Tools & Skills Demonstrated

**Tools**
- Microsoft Excel 2021
- Power Query
- Excel PivotTables
- Excel Charts and Interactive Dashboard

**Skills**
- Data cleaning and preparation
- Data transformation
- Calculated field creation
- Analytical thinking and problem-solving
- Business expense analysis
- Comparative analysis
- Data visualization
- Dashboard development
- Data validation and quality assessment
- Insight generation and business recommendations

## 14. Project Files

The repository includes the Excel workbook containing the complete analysis process and final dashboard.

**Executive Itinerary Cost Optimization GitHub.xlsx**

The workbook is organized into the following worksheets:

| Worksheet | Description |
|---|---|
| Project Overview | Introduces the project, objectives, dataset, tools, and workbook navigation. |
| Raw Data | Contains the original synthetic dataset. |
| Cleaned Data | Contains the prepared dataset, calculated fields, and validation calculations. |
| Trip Purpose Costs | Analyzes total trip costs by business purpose. |
| Hotel Category | Compares average hotel cost per night across categories. |
| Flight Comparison | Compares direct and connecting flights by cost and travel time. |
| Trip Priority | Examines trip costs across business priority levels. |
| Airline Comparison | Compares average flight costs across airlines. |
| Dashboard | Presents the key findings through an interactive Excel dashboard. |

## 15. Dashboard Preview

The interactive Excel dashboard provides a consolidated view of business travel expenses and key cost drivers.

It includes:

- Key expense summary and total trip count.
- Expense breakdown by category.
- Business travel cost comparisons.
- Interactive slicers for Trip Purpose and Destination.
- A Departure Date timeline for filtering the analysis.

A dashboard screenshot will be included here to provide a visual preview of the project.
