---
description: ''
layout: schema
name: SecFilingList
properties_list:
- description: ''
  name: total
  type: integer
- description: ''
  name: offset
  type: integer
- description: ''
  name: limit
  type: integer
- description: ''
  name: filings
  type: array
provider_name: Archrock
provider_slug: archrock
schema_file: json-schema/archrock-investor-relations-api-sec-filing-list-schema.json
slug: archrock-investor-relations-api-sec-filing-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/json-schema/archrock-investor-relations-api-sec-filing-list-schema.json\",\n  \"title\": \"SecFilingList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"filings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {},\n          \"type\": {},\n          \"filingDate\": {},\n          \"periodOfReport\": {},\n          \"description\": {},\n          \"secUrl\": {},\n          \"documentUrl\": {}\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/json-schema/archrock-investor-relations-api-sec-filing-list-schema.json
tags:
- Natural Gas
- Compression Services
- Oil And Gas
- Energy
- Industrial
- 'NYSE: AROC'
title: SecFilingList
---
