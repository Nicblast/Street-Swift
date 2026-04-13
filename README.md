# Street-Swift

![IMG_3475](https://github.com/user-attachments/assets/0f44cae6-31e9-4820-a6eb-a2dc0259ea93)
(Image generated with AI)
--
This analysis examines the first six months of StreetSwift, an urban mobility startup. The objective was to identify the root causes of high operational burn rates and lower-than-expected vehicle utilization across four primary city zones.

## Methodology

The raw data required a multi-stage Python transformation to ensure reporting accuracy:

The transformation includes:
--

* Data Integrity: Eliminated duplicate trip logs to prevent revenue overestimation.

* Logical Imputation: Reconstructed missing financial records using a $15/hr billing heuristic.

* Standardization: Synchronized disparate date formats to allow for accurate week-over-week trend analysis.

## Important note on methodology and data sources:

The data utilized in this project is a synthetic representation of car-sharing operations. It was generated using a custom script to simulate high-variance business scenarios, such as regional demand shifts and service-level fluctuations. This approach allows for a controlled validation of the Business Analyst's diagnostic framework without compromising sensitive proprietary or PII (Personally Identifiable Information) data.

## Business Problem

# Why is our fleet underperforming, and where exactly are we losing money?

To answer this for the CEO, the company has asked me to break that big question down into these four more specific sub-questions:

* Are the cars actually being driven?
* Why is our 'Total Bill' revenue lower than our projected growth?
* Why aren't people coming back for a second ride?

--

## Key Findings (Insights)

* The "Industrial Zone" Leak: This sector shows a 100% cancellation rate in the sample period. Fleet deployment in this zone currently generates zero ROI and incurs unnecessary logistics costs.

![IMG_3473](https://github.com/user-attachments/assets/269a1074-4c69-4cf2-9b78-47594da38f7d)


* Asset Underutilization: Average trip duration for "Economy" vehicles is under 1 hour. Given the fixed costs of maintenance and insurance per trip, short-duration rentals are currently operating at a net loss.

![IMG_3472](https://github.com/user-attachments/assets/359af46c-bf9c-4f69-b926-8b42b0d4662b)


* Luxury Quality Gap: "Luxury" tier vehicles report a 40% lower average user rating compared to "Electric" models, suggesting that the premium price point does not currently align with the vehicle condition or user experience.

![IMG_3474](https://github.com/user-attachments/assets/71e9bcbe-0f35-45ba-a451-c613007c46bf)

The result of the above findings results in the following:

![IMG_3470](https://github.com/user-attachments/assets/a1087a68-af35-4f89-8dd2-39f3a15b2a06)


## Strategic Recommendations

1.Fleet Relocation: Immediately transition 80% of the "Industrial Zone" fleet to the "Airport" and "Downtown" hubs where demand and completion rates are highest.

2.Pricing Restructuring: Implement a minimum booking fee (e.g., $20 minimum) to ensure that short-duration "micro-trips" remain profitable.

3.Tier Maintenance Audit: Conduct a physical audit of all "Luxury" assets to address the source of low user ratings and protect the brand’s premium positioning.


<img width="1536" height="1024" alt="IMG_3471" src="https://github.com/user-attachments/assets/7da774b4-9c85-4408-a90b-e63ca7d23290" />


## Constraints & future scope

* Sample Size Constraints: The current dataset provides a snapshot of 60–1,000 trips. While sufficient for identifying high-level trends, a larger longitudinal study (10,000+ rows) would be required to account for seasonal variations.

* Static Pricing Assumptions: The analysis assumes a fixed $15/hr billing rate. In a real-world scenario, dynamic pricing and varying insurance premiums per car model would add layers of complexity to the "Total Bill" calculation.

* Lack of Qualitative Feedback: While User_Rating gives a numerical score, the data lacks qualitative "Review Text." Without text data, we can only guess why a rating was low (e.g., was the car dirty, or was the app's GPS inaccurate?).

* Missing Operational Costs: The dataset focuses on revenue but lacks a "Cost" column (e.g., fuel, cleaning, parking permits). This limits the ability to calculate true Net Profit, allowing only for a "Gross Revenue" analysis.

* Geographic Granularity: "City Zones" (Downtown, Suburbs, etc.) are broad categories. Real-world mobility optimization usually requires specific GPS coordinates or "Hex-bins" to pinpoint the exact street corners where cars are actually being underutilized.

* Synthetic Homogeneity: Because the data is programmatically generated, it may lack the events (e.g., a major city marathon or a fleet-wide technical outage) that often disrupt real world startup operations.

--
