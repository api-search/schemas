---
description: A single economic indicator data point
layout: schema
name: EconomicDataPoint
properties_list:
- description: Date of the data point
  name: date
  type: string
- description: Indicator value for the period
  name: value
  type: string
provider_name: Alpha Vantage
provider_slug: alpha-vantage
schema_file: json-schema/alpha-vantage-economic_data_point-schema.json
slug: alpha-vantage-economic_data_point
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.alphavantage.co/schemas/alpha-vantage-economic_data_point-schema.json\",\n  \"title\": \"EconomicDataPoint\",\n  \"type\": \"object\",\n  \"description\": \"A single economic indicator data point\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the data point\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Indicator value for the period\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/json-schema/alpha-vantage-economic_data_point-schema.json
tags:
- Financial
- Market Data
- Stocks
- Technical Indicators
- Economic Data
- Sentiment Analysis
title: EconomicDataPoint
---
