---
description: A Program Increment (PI) in the Scaled Agile Framework representing a 8-12 week timebox for ART delivery.
layout: schema
name: SAFe Program Increment
properties_list:
- description: Unique program increment identifier
  name: id
  type: string
- description: PI name or number (e.g., PI-2026-Q2)
  name: name
  type: string
- description: PI start date
  name: start_date
  type: string
- description: PI end date
  name: end_date
  type: string
- description: Agile Release Train identifier
  name: art_id
  type: string
- description: PI objectives committed by teams
  name: objectives
  type: array
- description: Sprints/iterations within the PI
  name: iterations
  type: array
- description: Current PI status
  name: status
  type: string
provider_name: SAFe Agile
provider_slug: safe-agile
schema_file: json-schema/safe-agile-program-increment-schema.json
slug: safe-agile-program-increment
source_filename: safe-agile-program-increment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/safe-agile/main/json-schema/safe-agile-program-increment-schema.json\",\n  \"title\": \"SAFe Program Increment\",\n  \"description\": \"A Program Increment (PI) in the Scaled Agile Framework representing a 8-12 week timebox for ART delivery.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique program increment identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"PI name or number (e.g., PI-2026-Q2)\"\n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"PI start date\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"PI end date\"\n    },\n    \"art_id\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Agile Release Train identifier\"\n    },\n    \"objectives\": {\n      \"type\": \"array\",\n      \"description\": \"PI objectives committed by teams\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\"type\": \"string\"},\n          \"title\": {\"type\": \"string\"},\n          \"business_value\": {\"type\": \"integer\", \"minimum\": 1, \"maximum\": 10},\n          \"team_id\": {\"type\": \"string\"},\n          \"committed\": {\"type\": \"boolean\"}\n        }\n      }\n    },\n    \"iterations\": {\n      \"type\": \"array\",\n      \"description\": \"Sprints/iterations within the PI\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"number\": {\"type\": \"integer\"},\n          \"start_date\": {\"type\": \"string\", \"format\": \"date\"},\n          \"end_date\": {\"type\": \"string\", \"format\": \"date\"},\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\":\
  \ [\"development\", \"IP\"],\n            \"description\": \"Development iteration or Innovation and Planning\"\n          }\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"planned\", \"in_progress\", \"completed\"],\n      \"description\": \"Current PI status\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"start_date\", \"end_date\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/safe-agile/refs/heads/main/json-schema/safe-agile-program-increment-schema.json
tags:
- Agile
- Enterprise
- Framework
- Project Management
- Scaled Agile
- Lean Portfolio
- DevOps
title: SAFe Program Increment
---
