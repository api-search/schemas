---
description: List of monitors
layout: schema
name: MonitorListResponse
properties_list:
- description: ''
  name: monitors
  type: array
- description: ''
  name: totalCount
  type: integer
provider_name: BankruptcyWatch
provider_slug: bankruptcywatch
schema_file: json-schema/monitorlistresponse-schema.json
slug: monitorlistresponse
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bankruptcywatch/json-schema/monitorlistresponse-schema.json\",\n  \"title\": \"MonitorListResponse\",\n  \"type\": \"object\",\n  \"description\": \"List of monitors\",\n  \"properties\": {\n    \"monitors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Monitor\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bankruptcywatch/refs/heads/main/json-schema/monitorlistresponse-schema.json
tags:
- Bankruptcy
- Compliance
- Court Data
- Legal
- Lending
- PACER
title: MonitorListResponse
---
