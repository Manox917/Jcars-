# Jcars-
My main objective is to transform the raw JCars Logistics sales and operational dataset into a reliable Power BI business intelligence solution covering sales, revenue, profitability, vehicles, customers, branches, payments, deliveries, logistics, returns, cancellations and customer experience.
Cars Logistics Power BI Business Intelligence Project

# Dataset

276 rows

32 raw columns

 Raw grain: one supplied business record per row. Order ID is not a reliable unique key because duplicate/placeholder IDs exist and must be investigated.

## Data Quality

The audit identified issues including duplicate Order IDs, invalid dates, mixed currency formats, negative monetary values, invalid units, discounts above 100%, invalid vehicle years, inconsistent fuel/transmission/payment/delivery categories, inconsistent customer ratings, negative review counts and spelling/case variation across dimensions.


## Currency

Reporting currency: KES. Unmarked monetary values are treated as KES as required by the assessment. Explicit USD, EUR and ZAR values are converted using one consistent rate set from the Central Bank of Kenya:

USD 129.46 KES

EUR 148.46 KES

ZAR 7.96 KES

## Proposed Model

### Star-schema approach:

FactSales

DimDate

DimCustomer

DimVehicle

DimBranch

DimSalesRep

DimPayment

The final relationships should be one-to-many from dimensions to FactSales with a dedicated Date dimension.

### Dashboard Pages

Executive Dashboard

Sales & Profitability

Vehicle Performance

Customers & Sales Representatives

Branch & Geographic Performance

Payments & Revenue

Deliveries & Logistics

Returns, Cancellations & Customer Experience

Trends & Investigation

Interactivity

Include slicers, cross-filtering, a drill-through page, a report tooltip and page navigation.

## Important DAX

Core measures include Total Orders, Total Units Sold, Total Revenue, Total Cost, Gross Profit, Gross Profit Margin, Average Revenue per Unit, Logistics Cost, Logistics Cost %, Return Count, Cancellation Rate and Average Customer Rating.

## Important rule
Do not silently overwrite raw data. Keep raw fields and create cleaned/standardized analytical fields with documented rules and quality flags.
## Conclusion
The JCars project demonstrates the full BI workflow: raw data investigation, Power Query preparation, currency standardization, data modelling, DAX, interactive reporting, investigation and evidence-based management communication.
