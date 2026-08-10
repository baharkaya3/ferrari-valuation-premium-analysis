# Ferrari Valuation Premium Analysis: Automotive vs. Ultra-Luxury

## Project Overview
This project looks at how financial markets price Ferrari N.V. (RACE) using a Comparable Company Analysis (Comps) with two different groups. The main goal is to figure out if the market treats Ferrari like a regular car maker or like an ultra-luxury "Veblen" brand (which means high pricing power and artificial scarcity).

## Methodology & Data
I used historical financial data from 2023 to 2025. To get a good comparison, I built two different groups of peers:
1. **Automotive Cohort:** Porsche AG (ETR:P911), Aston Martin (LON:AML)
2. **Ultra-Luxury Cohort:** Hermès (EPA:RMS), Ferretti Group (BIT:YACHT), Brunello Cucinelli (BIT:BC)

### Financial Modeling & Currency Normalization
* **Currency Normalization:** Aston Martin reports in GBP, so I converted their numbers to EUR to make sure the comparisons are accurate.
    * *Income Statement items* (Revenue, EBITDA) were converted using the Annual Average Exchange Rate.
    * *Balance Sheet items* (Total Debt, Cash) and Market Cap were converted using the Year-End Spot Exchange Rate.
* **Valuation Metrics:** I mainly looked at the EV/EBITDA multiple, along with Gross Margin and EBITDA Margin to check operational efficiency.

## Key Findings

1. **Profitability Differences:** 
   The car makers have EBITDA margins around 16%-26%, but the luxury group is much higher, between 28%-48%. Ferrari’s EBITDA margin was about 38.8% in 2025, which shows they operate much more like a luxury brand than a typical automaker.

2. **The Valuation Premium:**
   The market gives the car makers an EV/EBITDA multiple of about 6x-9x. But luxury brands get much higher multiples, around 18x-33x. Ferrari’s 2025 EV/EBITDA multiple was ~20.9x, which proves the market gives them a premium for being a luxury status symbol, not just an industrial manufacturer.

3. **Data Correlation:**
   When you plot EBITDA Margins against EV/EBITDA multiples, there's a strong positive relationship ($R^2 = 0.947$) for the luxury group. Ferrari fits right on that luxury trendline, which backs up the main idea.

## Repository Structure
Everything is in a single Excel workbook (`.xlsx`) with three sheets:
* `Raw Data`: The original financial numbers from Stockanalysis and Yahoo Finance.
* `Calculations`: Where I did the FX conversions, Net Debt calculations, and figured out the multiples.
* `Dashboard`: A visual scatter plot showing Margins vs. Valuation and the trendlines for each group.

## Limitations
* **Ferretti's Lower Multiple:** Even though they make ultra-luxury yachts, Ferretti trades at lower multiples (~4x-5x). This shows that heavy manufacturing can lower a company's multiple, even if they are a luxury brand.
* **Aston Martin's EBITDA:** Aston Martin had a big drop in EBITDA, which made their EV/EBITDA multiple jump around a lot. This adds some noise when looking at the automotive group averages.
## ⚠️ Limitations & Nuances
* **Ferretti's Industrial Nature:** Despite being an ultra-luxury yacht manufacturer, Ferretti trades at lower multiples (~4x-5x), indicating that heavy-industrial production constraints can weigh down pure "Veblen" status multipliers.
* **Aston Martin's EBITDA Volatility:** A sharp decline in Aston Martin's EBITDA resulted in outsized EV/EBITDA multiplier volatility, which introduces noise when calculating automotive cohort averages.
