---
description: ''
layout: schema
name: SafetyInfo
properties_list:
- description: Country slug
  name: country
  type: string
- description: ''
  name: overallRating
  type: string
- description: Advisory level (1=normal, 4=do not travel)
  name: advisoryLevel
  type: integer
- description: ''
  name: categories
  type: object
- description: Additional safety notes
  name: notes
  type: string
provider_name: Basetrip
provider_slug: basetrip
schema_file: json-schema/safetyinfo.json
slug: safetyinfo
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/safetyinfo.json\",\n  \"title\": \"SafetyInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country slug\"\n    },\n    \"overallRating\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Safe\",\n        \"Moderate\",\n        \"Risky\",\n        \"High Risk\",\n        \"Extreme\"\n      ]\n    },\n    \"advisoryLevel\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 4,\n      \"description\": \"Advisory level (1=normal, 4=do not travel)\"\n    },\n    \"categories\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"crime\": {\n          \"type\": \"string\"\n        },\n        \"terrorism\": {\n          \"type\": \"string\"\n        },\n        \"naturalDisasters\": {\n\
  \          \"type\": \"string\"\n        }\n      }\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Additional safety notes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/safetyinfo.json
tags:
- Cities
- Countries
- Health
- Safety
- Travel
- Visa
title: SafetyInfo
---
