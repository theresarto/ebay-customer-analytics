# Data Dictionary - eBay Beauty Products Dataset

## Overview
Anonymized sample of eBay beauty product sales (March 2023 - February 2025)

## Columns

| Column | Type | Description | Example |
|--------|------|-------------|---------|
| Sales record number | int | Unique sale ID | 12345 |
| Order number | str | eBay order ID | 01-23456-78901 |
| Buyer username | str | Anonymized customer ID | user_a3f4b2c1 |
| Buyer postcode | str | Generalized UK postcode | SW1 |
| Item number | str | Anonymized item ID | item_abc123def4 |
| Item title | str | Product name/description | Kojie San Soap 135g x 2 |
| Sold via Promoted listings | str | Promotion used (Yes/No) | Yes |
| Quantity | int | Number of packs/items purchased | 3 |
| Sold for | str | Total transaction price (GBP) | £25.47 |
| Sale date | str | Transaction date | 15-Mar-24 |
| Brand | str | Product brand | Kojie San |
| Discount_Percentage | int | Multi-buy discount applied | 15 |
| Product_Category | str | Product type | Soap |
| Product_Size | str | Size from title | 135g |
| Unit_Size | str | Size per unit | 135g |
| Pack_Count | int | Units per pack | 2 |
| Total_Size | str | Total product size | 270g |
| Is_Multipack | bool | Pre-packaged multiple units | True |
| Total_Units | int | Total individual units | 6 |

## Privacy Notes
- Customer usernames: MD5 hashed
- Postcodes: Generalized to area level  
- Prices: ±5% random variation applied
- Dates: Shifted ±30 days
- Item numbers: MD5 hashed

## Pricing Structure
- 1 item: No discount
- 2 items: 10% discount
- 3 items: 15% discount  
- 4+ items: 20% discount