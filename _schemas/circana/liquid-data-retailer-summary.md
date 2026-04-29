---
description: Retailer summary record
layout: schema
name: RetailerSummary
properties_list:
- description: Unique retailer identifier
  name: retailer_id
  type: string
- description: Retailer name
  name: name
  type: string
- description: Primary retail channel
  name: channel
  type: string
- description: Number of store locations
  name: store_count
  type: integer
- description: Geographic coverage level
  name: geographic_coverage
  type: string
provider_name: Circana
provider_slug: circana
schema_file: json-schema/liquid-data-retailer-summary-schema.json
slug: liquid-data-retailer-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-retailer-summary-schema.json\",\n  \"title\": \"RetailerSummary\",\n  \"description\": \"Retailer summary record\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"retailer_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique retailer identifier\",\n      \"example\": \"ret-500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Retailer name\",\n      \"example\": \"Example Market\"\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"description\": \"Primary retail channel\",\n      \"example\": \"grocery\"\n    },\n    \"store_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of store locations\",\n      \"example\": 450\n    },\n    \"geographic_coverage\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Geographic coverage level\",\n      \"example\": \"national\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-retailer-summary-schema.json
tags:
- Analytics
- Consumer Data
- Market Research
- Retail
- CPG
- Point Of Sale
- Consumer Insights
- Business Intelligence
title: RetailerSummary
---
