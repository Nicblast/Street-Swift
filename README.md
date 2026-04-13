# Street-Swift
This analysis examines the first six months of StreetSwift, an urban mobility startup. The objective was to identify the root causes of high operational burn rates and lower-than-expected vehicle utilization across four primary city zones.

## Methodology

The raw data required a multi-stage Python transformation to ensure reporting accuracy:

The transformation includes:
--

* Data Integrity: Eliminated duplicate trip logs to prevent revenue overestimation.

* Logical Imputation: Reconstructed missing financial records using a $15/hr billing heuristic.

* Standardization: Synchronized disparate date formats to allow for accurate week-over-week trend analysis.

## Problem

# "Why is our fleet underperforming, and where exactly are we losing money?"

To answer this for the CEO, the company has asked me to break that big question down into these four more specific sub-questions:

* Are the cars actually being driven?
* Why is our 'Total Bill' revenue lower than our projected growth?
* Why aren't people coming back for a second ride?

--

## Key Findings (Insights)

* The "Industrial Zone" Leak: This sector shows a 100% cancellation rate in the sample period. Fleet deployment in this zone currently generates zero ROI and incurs unnecessary logistics costs.

* Asset Underutilization: Average trip duration for "Economy" vehicles is under 1 hour. Given the fixed costs of maintenance and insurance per trip, short-duration rentals are currently operating at a net loss.

* Luxury Quality Gap: "Luxury" tier vehicles report a 40% lower average user rating compared to "Electric" models, suggesting that the premium price point does not currently align with the vehicle condition or user experience.

## Strategic Recommendations

1.Fleet Relocation: Immediately transition 80% of the "Industrial Zone" fleet to the "Airport" and "Downtown" hubs where demand and completion rates are highest.

2.Pricing Restructuring: Implement a minimum booking fee (e.g., $20 minimum) to ensure that short-duration "micro-trips" remain profitable.

3.Tier Maintenance Audit: Conduct a physical audit of all "Luxury" assets to address the source of low user ratings and protect the brand’s premium positioning.

