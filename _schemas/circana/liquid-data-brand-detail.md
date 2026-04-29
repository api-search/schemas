---
description: Detailed brand information
layout: schema
name: BrandDetail
properties_list:
- description: Unique brand identifier
  name: brand_id
  type: string
- description: Brand name
  name: name
  type: string
- description: Manufacturer or parent company name
  name: manufacturer
  type: string
- description: Categories the brand is present in
  name: categories
  type: array
- description: Number of UPCs under this brand
  name: upc_count
  type: integer
- description: Brand market presence information
  name: market_presence
  type: object
provider_name: Circana
provider_slug: circana
schema_file: json-schema/liquid-data-brand-detail-schema.json
slug: liquid-data-brand-detail
source_filename: liquid-data-brand-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-brand-detail-schema.json\",\n  \"title\": \"BrandDetail\",\n  \"description\": \"Detailed brand information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique brand identifier\",\n      \"example\": \"brand-500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Brand name\",\n      \"example\": \"Example Cola\"\n    },\n    \"manufacturer\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer or parent company name\",\n      \"example\": \"Example Corp\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"description\": \"Categories the brand is present in\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"upc_count\": {\n   \
  \   \"type\": \"integer\",\n      \"description\": \"Number of UPCs under this brand\",\n      \"example\": 45\n    },\n    \"market_presence\": {\n      \"type\": \"object\",\n      \"description\": \"Brand market presence information\",\n      \"properties\": {\n        \"channels\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of retail channels with distribution\"\n        },\n        \"retailers\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of retailers carrying the brand\"\n        },\n        \"geographic_coverage\": {\n          \"type\": \"string\",\n          \"description\": \"Geographic coverage level\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-brand-detail-schema.json
tags:
- Analytics
- Consumer Data
- Market Research
- Retail
- CPG
- Point Of Sale
- Consumer Insights
- Business Intelligence
title: BrandDetail
---
