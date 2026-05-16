GITHUB URL:
https://github.com/pdagur/Berkeley_Module_11.2_Practical_Exam2/blob/main/Chap11-CarPrice_usedCar.ipynb



# Used Car Price Analysis

## Overview
This project analyzes more than 426000 used car listings to identify the key factors that influence vehicle pricing. The objective is to support dealerships in making informed decisions about pricing and inventory selection.

---

## Pricing Hypothesis

Used car prices are primarily determined by depreciation driven by age and mileage. Additional adjustments come from utility, brand perception, and risk related attributes.

---

## Key Drivers

### 1. Depreciation
Age and mileage explain the largest share of price variation. Depreciation is not linear, with the steepest decline occurring in the first few years of a vehicle's life.

### 2. Utility and Capability
Vehicles with higher functional value such as diesel engines, four wheel drive, and pickup configurations tend to retain value better. These characteristics signal durability and long term usefulness.

### 3. Brand Perception
Premium brands command higher prices. Brand serves as a proxy for quality, reliability, and overall market perception.

### 4. Condition and Risk Indicators
Vehicles with clean titles and good condition are priced higher. Cars with salvage or damaged titles are discounted due to increased risk.

### 5. Segment Dynamics
Economy vehicles tend to depreciate faster due to high supply and lower differentiation. Trucks and specialized vehicles generally maintain stronger pricing.

---

## Modeling Approach

The dataset was cleaned from approximately 427000 records to about 330000 usable observations. Feature engineering included age calculation, mileage filtering, and encoding of categorical variables.

The following models were evaluated:
- Linear and Ridge Regression with an R squared of approximately 0.70
- Gradient Boosting with an R squared of approximately 0.82

Gradient Boosting performs better because it captures non linear relationships and feature interactions more effectively.

---

## Key Insight

Used car pricing follows a non linear depreciation curve that is adjusted by functional value, brand reputation, and risk indicators such as condition and title status.

---

## Limitations

The dataset reflects listing prices rather than actual transaction prices. Some important attributes such as trim level are not included. Regional differences are only partially captured.

---

## Next Steps

Future improvements include modeling log transformed prices, adding interaction terms such as age and brand, building segment specific models, and incorporating additional features such as trim level.
