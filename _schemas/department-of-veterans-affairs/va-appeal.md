---
description: An appeal, supplemental claim, or higher-level review tracked through VA's appeals modernization process.
layout: schema
name: VA Appeal
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Department of Veterans Affairs (VA)
provider_slug: department-of-veterans-affairs
schema_file: json-schema/va-appeal-schema.json
slug: va-appeal
source_filename: va-appeal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/department-of-veterans-affairs/schemas/appeal.json\",\n  \"title\": \"VA Appeal\",\n  \"description\": \"An appeal, supplemental claim, or higher-level review tracked through VA's appeals modernization process.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\", \"attributes\"],\n  \"properties\": {\n    \"id\": { \"type\": \"string\" },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"legacyAppeal\", \"appeal\", \"supplementalClaim\", \"higherLevelReview\"]\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"appealIds\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n        \"updated\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"programArea\": { \"type\": \"string\" },\n        \"description\": { \"type\": \"string\" },\n        \"type\": { \"type\": \"string\"\
  \ },\n        \"aoj\": { \"type\": \"string\", \"enum\": [\"vba\", \"vha\", \"nca\", \"other\"] },\n        \"location\": { \"type\": \"string\", \"enum\": [\"aoj\", \"bva\"] },\n        \"status\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": { \"type\": \"string\" },\n            \"details\": { \"type\": \"object\" }\n          }\n        },\n        \"events\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": { \"type\": \"string\" },\n              \"date\": { \"type\": \"string\", \"format\": \"date\" }\n            }\n          }\n        },\n        \"issues\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"active\": { \"type\": \"boolean\" },\n              \"description\": { \"type\": \"string\" },\n              \"diagnosticCode\": { \"type\":\
  \ [\"string\", \"null\"] },\n              \"lastAction\": { \"type\": [\"string\", \"null\"] },\n              \"date\": { \"type\": [\"string\", \"null\"], \"format\": \"date\" }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/department-of-veterans-affairs/refs/heads/main/json-schema/va-appeal-schema.json
tags:
- Federal Government
- Healthcare
- Veterans
title: VA Appeal
---
