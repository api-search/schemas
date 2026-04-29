---
description: Individual point-of-sale data record
layout: schema
name: POSRecord
properties_list:
- description: Time period identifier
  name: period
  type: string
- description: Product category name
  name: category
  type: string
- description: Brand name
  name: brand
  type: string
- description: Universal Product Code
  name: upc
  type: string
- description: Total dollar sales for the period
  name: dollar_sales
  type: number
- description: Total unit sales for the period
  name: unit_sales
  type: integer
- description: Total volume sales (equivalent units)
  name: volume_sales
  type: number
- description: Average selling price
  name: avg_price
  type: number
- description: Percentage of stores carrying the product
  name: distribution_pct
  type: number
provider_name: Circana
provider_slug: circana
schema_file: json-schema/liquid-data-pos-record-schema.json
slug: liquid-data-pos-record
source_filename: liquid-data-pos-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-pos-record-schema.json\",\n  \"title\": \"POSRecord\",\n  \"description\": \"Individual point-of-sale data record\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"period\": {\n      \"type\": \"string\",\n      \"description\": \"Time period identifier\",\n      \"example\": \"2026-W01\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Product category name\",\n      \"example\": \"Beverages\"\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Brand name\",\n      \"example\": \"Example Brand\"\n    },\n    \"upc\": {\n      \"type\": \"string\",\n      \"description\": \"Universal Product Code\",\n      \"example\": \"012345678901\"\n    },\n    \"dollar_sales\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n\
  \      \"description\": \"Total dollar sales for the period\",\n      \"example\": 125340.50\n    },\n    \"unit_sales\": {\n      \"type\": \"integer\",\n      \"description\": \"Total unit sales for the period\",\n      \"example\": 45230\n    },\n    \"volume_sales\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total volume sales (equivalent units)\",\n      \"example\": 67845.0\n    },\n    \"avg_price\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Average selling price\",\n      \"example\": 2.77\n    },\n    \"distribution_pct\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Percentage of stores carrying the product\",\n      \"example\": 85.3\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-pos-record-schema.json
tags:
- Analytics
- Consumer Data
- Market Research
- Retail
- CPG
- Point Of Sale
- Consumer Insights
- Business Intelligence
title: POSRecord
---
