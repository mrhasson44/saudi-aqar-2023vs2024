# Saudi Arabia Real Estate Analysis 2022Q1 & 2023Q1

## Project Overview

<<<<<<< HEAD
This project performs a comprehensive exploratory data analysis (EDA) on real estate transaction data from Saudi Arabia and foucsing on three ragion [Riyadh,Mecca,Eastern Province], comparing the first quarters of 2022 and 2023. The analysis extracts meaningful insights about market trends, property valuations, geographic patterns, and market segmentation to understand how the Saudi real estate market evolved during this period.
=======
This project performs a comprehensive exploratory data analysis (EDA) on real estate transaction data from Saudi Arabia, comparing the first quarters of 2022 and 2023. The analysis extracts meaningful insights about market trends, property valuations, geographic patterns, and market segmentation to understand how the Saudi real estate market evolved during this period.
>>>>>>> 48d9b0cad336624412841d8916b6035fb84ab5ee

## Dataset

The analysis uses two cleaned datasets:
- `real_estate_2022Q1.csv`: Real estate transactions from Q1 2022
- `real_estate_2023Q1.csv`: Real estate transactions from Q1 2023

Each dataset contains the following columns:
- `ref_num`: Reference number for the transaction
- `area`: Area/neighborhood
- `city`: City name
- `district`: District name
- `Mukatat`: Administrative division
- `piece_num`: Property identifier
- `date`: Transaction date
- `property_classification`: Classification of the property
- `property_type`: Type of property (residential, commercial, etc.)
- `number_of_properties`: Number of properties in the transaction
- `price`: Transaction price in Saudi Riyal (SAR)
- `space`: Property size in square meters
- `Price_per_square_meter`: Price divided by space (SAR/m²)

## Data Preparation

During our exploratory data analysis (EDA), we applied the following data preparation steps:

1. **Single Property Transactions**: We removed any rows where more than one plot of land was for sale (`number_of_properties > 1`), as the price often varies in these cases and could skew our analysis.

2. **Focus on Major Regions**: We kept only transactions from the three largest regions:
   - Riyadh
   - Eastern Province
   - Makkah Al-Mukarramah

These preprocessing steps allowed us to perform more accurate and focused analyses on the Saudi real estate market.

## Key Insights

Our analysis explores five key insights:

1. **Price Trend Analysis**: Year-over-year comparison of property prices and price per square meter across different cities and districts.

2. **Property Type Performance**: Analysis of how different property types performed in terms of price and transaction volume between 2022Q1 and 2023Q1.

3. **Geographic Distribution**: Examination of transaction density and average prices across different cities and districts, identifying high-growth areas.

4. **Space Utilization**: Analysis of the relationship between property size and price per square meter to understand value variations across different property sizes.

5. **Market Segmentation**: Distribution of properties across different price segments and how this distribution changed between the two periods.

## Tools and Libraries

To run the analysis scripts, you'll need:

- Python 3.8+
- pandas
- numpy
- matplotlib
- seaborn
- arabic-reshaper
- python-bidi

Install required packages:
```bash
pip install pandas numpy matplotlib seaborn arabic-reshaper python-bidi
```

## Directory Structure

```
saudi-real-estate-analysis/
│
├── data/
│   ├── 2022_q1.csv             # Original data files
|   ├── 2023_q1.csv             # Original data files
│   ├── Cleaneddata2022.csv     # Cleaned and transformed data
│   ├── Cleaneddata2023.csv     # Cleaned and transformed data
│
├── notebooks/
│   ├── insight_ghada.ipynb  
│   ├── insight_Ezdhar.ipynb       
|
├── StreamLit       
│
├──Real Estate Analysis              
│
└── READ-ME.md            
```

## Usage

1. Clone the repository:
```bash
git clone https://github.com/AI-bootcamp/data-science-project-team2p2ds.git 
cd saudi-real-estate-analysis
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run the main analysis script:
```bash
python scripts/main_analysis.py
```

Alternatively, run individual insight scripts:
```bash
python scripts/price_trend_analysis.py
python scripts/market_segmentation.py
# etc.
```

## Data Source

The Saudi Open Data Portal

## Data Visualization

The project includes various visualizations:
- Bar charts comparing 2022Q1 and 2023Q1 metrics
- Scatter plots examining price-space relationships
- Segment distribution analysis charts
- Arabic-text compatible visualizations for district and city data

## Results

The analysis provides insights into:
- Year-over-year price changes across different market segments
- Geographic areas with highest value growth
- Property types with strongest and weakest performance
- Space-price relationships and optimal property sizes
- Shifts in market segment distribution

## Future Work

Potential extensions to this analysis:
- Incorporate additional quarters to establish longer-term trends
- Add demographic data to correlate with property preferences
- Perform predictive modeling to forecast future price trends
- Analyze the impact of government policies on the real estate market

## Team Members

- Ezdhar Altamimi 
- Ghada Alamri
- OMAR ALSURAIA
- Abdullah AlDayel
- AbdulMohsen Aldougayyim