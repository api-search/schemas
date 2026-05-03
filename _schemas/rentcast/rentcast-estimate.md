---
description: An automated valuation model (AVM) estimate for a property's rent or sale value, with comparable properties
layout: schema
name: RentCast Property Estimate
properties_list:
- description: Estimated rent or sale price in USD
  name: price
  type: number
- description: Low end of the estimated price range in USD
  name: priceRangeLow
  type: number
- description: High end of the estimated price range in USD
  name: priceRangeHigh
  type: number
- description: Latitude of the subject property
  name: latitude
  type: number
- description: Longitude of the subject property
  name: longitude
  type: number
- description: List of comparable properties used in the estimate
  name: comparables
  type: array
provider_name: RentCast
provider_slug: rentcast
schema_file: json-schema/rentcast-estimate-schema.json
slug: rentcast-estimate
source_filename: rentcast-estimate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api.rentcast.io/schemas/estimate\",\n  \"title\": \"RentCast Property Estimate\",\n  \"description\": \"An automated valuation model (AVM) estimate for a property's rent or sale value, with comparable properties\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Estimated rent or sale price in USD\",\n      \"example\": 2200\n    },\n    \"priceRangeLow\": {\n      \"type\": \"number\",\n      \"description\": \"Low end of the estimated price range in USD\",\n      \"example\": 1980\n    },\n    \"priceRangeHigh\": {\n      \"type\": \"number\",\n      \"description\": \"High end of the estimated price range in USD\",\n      \"example\": 2420\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"description\": \"Latitude of the subject property\"\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n \
  \     \"description\": \"Longitude of the subject property\"\n    },\n    \"comparables\": {\n      \"type\": \"array\",\n      \"description\": \"List of comparable properties used in the estimate\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"string\" },\n          \"formattedAddress\": { \"type\": \"string\" },\n          \"propertyType\": { \"type\": \"string\" },\n          \"bedrooms\": { \"type\": \"number\" },\n          \"bathrooms\": { \"type\": \"number\" },\n          \"squareFootage\": { \"type\": \"integer\" },\n          \"price\": {\n            \"type\": \"number\",\n            \"description\": \"Listed or sold price of the comparable\"\n          },\n          \"distance\": {\n            \"type\": \"number\",\n            \"description\": \"Distance from subject property in miles\"\n          },\n          \"daysOnMarket\": {\n            \"type\": \"integer\",\n            \"description\": \"Number\
  \ of days the comparable was listed\"\n          },\n          \"listedDate\": {\n            \"type\": \"string\",\n            \"format\": \"date\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rentcast/refs/heads/main/json-schema/rentcast-estimate-schema.json
tags:
- Real Estate
- Property Data
- Valuation
- Rental Market
- AVM
title: RentCast Property Estimate
---
