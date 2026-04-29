---
description: ''
layout: schema
name: FilingList
properties_list:
- description: ''
  name: filings
  type: array
- description: Total number of filings
  name: totalCount
  type: integer
provider_name: Arch Coal
provider_slug: arch-coal
schema_file: json-schema/arch-coal-investor-relations-api-filing-list-schema.json
slug: arch-coal-investor-relations-api-filing-list
source_filename: arch-coal-investor-relations-api-filing-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"filings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {},\n          \"date\": {},\n          \"title\": {},\n          \"url\": {}\n        }\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of filings\",\n      \"example\": 25\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arch-coal/refs/heads/main/json-schema/arch-coal-investor-relations-api-filing-list-schema.json\",\n  \"title\": \"FilingList\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arch-coal/refs/heads/main/json-schema/arch-coal-investor-relations-api-filing-list-schema.json
tags:
- Mining
- Coal
- Metallurgical Coal
- Thermal Coal
- Energy
- Fortune 500
title: FilingList
---
