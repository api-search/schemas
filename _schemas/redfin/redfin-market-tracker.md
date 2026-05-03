---
description: A single record from a Redfin Data Center market tracker dataset, representing housing market metrics for a specific region, property type, and time period.
layout: schema
name: Redfin Market Tracker Record
properties_list:
- description: Start date of the measurement period.
  name: period_begin
  type: string
- description: End date of the measurement period.
  name: period_end
  type: string
- description: Duration type of the period.
  name: period_duration
  type: string
- description: Geographic level of the region.
  name: region_type
  type: string
- description: Numeric identifier for the region type.
  name: region_type_id
  type: integer
- description: Numeric identifier for the data table.
  name: table_id
  type: integer
- description: Whether the data has been seasonally adjusted.
  name: is_seasonally_adjusted
  type: boolean
- description: Name of the geographic region.
  name: region
  type: string
- description: City name, if applicable to the region level.
  name: city
  type: string
- description: State name.
  name: state
  type: string
- description: Two-letter US state code.
  name: state_code
  type: string
- description: Property type segment for the metrics.
  name: property_type
  type: string
- description: Median sale price for the period and region in USD.
  name: median_sale_price
  type: number
- description: Year-over-year change in median sale price as a decimal (e.g., 0.05 for 5% increase).
  name: median_sale_price_yoy
  type: number
- description: Median list price for the period and region in USD.
  name: median_list_price
  type: number
- description: Year-over-year change in median list price as a decimal.
  name: median_list_price_yoy
  type: number
- description: Median price per square foot in USD.
  name: median_ppsf
  type: number
- description: Year-over-year change in median price per square foot as a decimal.
  name: median_ppsf_yoy
  type: number
- description: Number of homes sold during the period.
  name: homes_sold
  type: integer
- description: Year-over-year change in homes sold as a decimal.
  name: homes_sold_yoy
  type: number
- description: Number of pending sales during the period.
  name: pending_sales
  type: integer
- description: Year-over-year change in pending sales as a decimal.
  name: pending_sales_yoy
  type: number
- description: Number of new listings added during the period.
  name: new_listings
  type: integer
- description: Year-over-year change in new listings as a decimal.
  name: new_listings_yoy
  type: number
- description: Total active inventory at the end of the period.
  name: inventory
  type: integer
- description: Year-over-year change in inventory as a decimal.
  name: inventory_yoy
  type: number
- description: Months of supply based on current sales pace.
  name: months_of_supply
  type: number
- description: Year-over-year change in months of supply as a decimal.
  name: months_of_supply_yoy
  type: number
- description: Median days on market.
  name: median_dom
  type: integer
- description: Year-over-year change in median days on market as a decimal.
  name: median_dom_yoy
  type: number
- description: Average sale-to-list price ratio (e.g., 1.02 means 2% above list).
  name: avg_sale_to_list
  type: number
- description: Year-over-year change in average sale-to-list ratio.
  name: avg_sale_to_list_yoy
  type: number
- description: Proportion of homes sold above list price (0 to 1).
  name: sold_above_list
  type: number
- description: Year-over-year change in proportion sold above list.
  name: sold_above_list_yoy
  type: number
- description: Proportion of listings with price drops (0 to 1).
  name: price_drops
  type: number
- description: Year-over-year change in proportion of price drops.
  name: price_drops_yoy
  type: number
- description: Proportion of listings that went off market within two weeks (0 to 1).
  name: off_market_in_two_weeks
  type: number
- description: Year-over-year change in proportion going off market in two weeks.
  name: off_market_in_two_weeks_yoy
  type: number
provider_name: Redfin
provider_slug: redfin
schema_file: json-schema/redfin-market-tracker-schema.json
slug: redfin-market-tracker
source_filename: redfin-market-tracker-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://redfin.com/schemas/redfin/market-tracker.json\",\n  \"title\": \"Redfin Market Tracker Record\",\n  \"description\": \"A single record from a Redfin Data Center market tracker dataset, representing housing market metrics for a specific region, property type, and time period.\",\n  \"type\": \"object\",\n  \"required\": [\"period_begin\", \"period_end\", \"region_type\", \"region\"],\n  \"properties\": {\n    \"period_begin\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Start date of the measurement period.\"\n    },\n    \"period_end\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"End date of the measurement period.\"\n    },\n    \"period_duration\": {\n      \"type\": \"string\",\n      \"enum\": [\"weekly\", \"monthly\"],\n      \"description\": \"Duration type of the period.\"\n    },\n    \"region_type\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\"national\", \"metro\", \"state\", \"county\", \"city\", \"zip_code\", \"neighborhood\"],\n      \"description\": \"Geographic level of the region.\"\n    },\n    \"region_type_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric identifier for the region type.\"\n    },\n    \"table_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric identifier for the data table.\"\n    },\n    \"is_seasonally_adjusted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the data has been seasonally adjusted.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the geographic region.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City name, if applicable to the region level.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State name.\"\n    },\n    \"state_code\": {\n      \"type\": \"string\"\
  ,\n      \"minLength\": 2,\n      \"maxLength\": 2,\n      \"pattern\": \"^[A-Z]{2}$\",\n      \"description\": \"Two-letter US state code.\"\n    },\n    \"property_type\": {\n      \"type\": \"string\",\n      \"enum\": [\"All Residential\", \"Single Family Residential\", \"Condo/Co-op\", \"Townhouse\", \"Multi-Family\"],\n      \"description\": \"Property type segment for the metrics.\"\n    },\n    \"median_sale_price\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Median sale price for the period and region in USD.\"\n    },\n    \"median_sale_price_yoy\": {\n      \"type\": \"number\",\n      \"description\": \"Year-over-year change in median sale price as a decimal (e.g., 0.05 for 5% increase).\"\n    },\n    \"median_list_price\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Median list price for the period and region in USD.\"\n    },\n    \"median_list_price_yoy\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Year-over-year change in median list price as a decimal.\"\n    },\n    \"median_ppsf\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Median price per square foot in USD.\"\n    },\n    \"median_ppsf_yoy\": {\n      \"type\": \"number\",\n      \"description\": \"Year-over-year change in median price per square foot as a decimal.\"\n    },\n    \"homes_sold\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of homes sold during the period.\"\n    },\n    \"homes_sold_yoy\": {\n      \"type\": \"number\",\n      \"description\": \"Year-over-year change in homes sold as a decimal.\"\n    },\n    \"pending_sales\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of pending sales during the period.\"\n    },\n    \"pending_sales_yoy\": {\n      \"type\": \"number\",\n      \"description\": \"Year-over-year change in pending sales as a decimal.\"\n    },\n    \"new_listings\"\
  : {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of new listings added during the period.\"\n    },\n    \"new_listings_yoy\": {\n      \"type\": \"number\",\n      \"description\": \"Year-over-year change in new listings as a decimal.\"\n    },\n    \"inventory\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Total active inventory at the end of the period.\"\n    },\n    \"inventory_yoy\": {\n      \"type\": \"number\",\n      \"description\": \"Year-over-year change in inventory as a decimal.\"\n    },\n    \"months_of_supply\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Months of supply based on current sales pace.\"\n    },\n    \"months_of_supply_yoy\": {\n      \"type\": \"number\",\n      \"description\": \"Year-over-year change in months of supply as a decimal.\"\n    },\n    \"median_dom\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\"\
  : \"Median days on market.\"\n    },\n    \"median_dom_yoy\": {\n      \"type\": \"number\",\n      \"description\": \"Year-over-year change in median days on market as a decimal.\"\n    },\n    \"avg_sale_to_list\": {\n      \"type\": \"number\",\n      \"description\": \"Average sale-to-list price ratio (e.g., 1.02 means 2% above list).\"\n    },\n    \"avg_sale_to_list_yoy\": {\n      \"type\": \"number\",\n      \"description\": \"Year-over-year change in average sale-to-list ratio.\"\n    },\n    \"sold_above_list\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Proportion of homes sold above list price (0 to 1).\"\n    },\n    \"sold_above_list_yoy\": {\n      \"type\": \"number\",\n      \"description\": \"Year-over-year change in proportion sold above list.\"\n    },\n    \"price_drops\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Proportion of listings with price\
  \ drops (0 to 1).\"\n    },\n    \"price_drops_yoy\": {\n      \"type\": \"number\",\n      \"description\": \"Year-over-year change in proportion of price drops.\"\n    },\n    \"off_market_in_two_weeks\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Proportion of listings that went off market within two weeks (0 to 1).\"\n    },\n    \"off_market_in_two_weeks_yoy\": {\n      \"type\": \"number\",\n      \"description\": \"Year-over-year change in proportion going off market in two weeks.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/json-schema/redfin-market-tracker-schema.json
tags:
- CSV Export
- GIS
- Home Values
- Housing Market
- Listings
- Property Data
- Real Estate
title: Redfin Market Tracker Record
---
