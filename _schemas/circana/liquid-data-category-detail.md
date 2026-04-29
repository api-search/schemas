---
description: Detailed category information
layout: schema
name: CategoryDetail
properties_list:
- description: Unique category identifier
  name: category_id
  type: string
- description: Category name
  name: name
  type: string
- description: Category description
  name: description
  type: string
- description: Parent category identifier
  name: parent_id
  type: string
- description: Industry vertical
  name: industry
  type: string
- description: Depth level in the category hierarchy
  name: level
  type: integer
- description: Direct subcategories
  name: subcategories
  type: array
- description: Data availability and coverage information
  name: data_coverage
  type: object
provider_name: Circana
provider_slug: circana
schema_file: json-schema/liquid-data-category-detail-schema.json
slug: liquid-data-category-detail
source_filename: liquid-data-category-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-category-detail-schema.json\",\n  \"title\": \"CategoryDetail\",\n  \"description\": \"Detailed category information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique category identifier\",\n      \"example\": \"cpg-beverages\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Category name\",\n      \"example\": \"Beverages\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Category description\",\n      \"example\": \"All beverage categories including carbonated, juice, water, and energy drinks\"\n    },\n    \"parent_id\": {\n      \"type\": \"string\",\n      \"description\": \"Parent category identifier\",\n      \"example\": \"cpg\"\n    },\n\
  \    \"industry\": {\n      \"type\": \"string\",\n      \"description\": \"Industry vertical\",\n      \"example\": \"cpg\"\n    },\n    \"level\": {\n      \"type\": \"integer\",\n      \"description\": \"Depth level in the category hierarchy\",\n      \"example\": 2\n    },\n    \"subcategories\": {\n      \"type\": \"array\",\n      \"description\": \"Direct subcategories\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"category_id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"parent_id\": {\n            \"type\": \"string\"\n          },\n          \"industry\": {\n            \"type\": \"string\"\n          },\n          \"level\": {\n            \"type\": \"integer\"\n          },\n          \"subcategory_count\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"data_coverage\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"Data availability and coverage information\",\n      \"properties\": {\n        \"pos_available\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether POS data is available\"\n        },\n        \"panel_available\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether consumer panel data is available\"\n        },\n        \"earliest_date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Earliest available data date\"\n        },\n        \"latest_date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Latest available data date\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-category-detail-schema.json
tags:
- Analytics
- Consumer Data
- Market Research
- Retail
- CPG
- Point Of Sale
- Consumer Insights
- Business Intelligence
title: CategoryDetail
---
