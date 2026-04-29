---
description: DayOfWeekRestriction schema from Adyen API
layout: schema
name: DayOfWeekRestriction
properties_list:
- description: Defines how the condition must be evaluated.
  name: operation
  type: string
- description: 'List of days of the week. Possible values: **monday**, **tuesday**, **wednesday**, **thursday**, **friday**, **saturday**, **sunday**.'
  name: value
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-day-of-week-restriction-schema.json
slug: configuration-day-of-week-restriction
source_filename: configuration-day-of-week-restriction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-day-of-week-restriction-schema.json\",\n  \"title\": \"DayOfWeekRestriction\",\n  \"description\": \"DayOfWeekRestriction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"description\": \"Defines how the condition must be evaluated.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"List of days of the week.\\n\\nPossible values: **monday**, **tuesday**, **wednesday**, **thursday**, **friday**, **saturday**, **sunday**.\\n\\n\",\n      \"items\": {\n        \"enum\": [\n          \"friday\",\n          \"monday\",\n          \"saturday\",\n          \"sunday\",\n          \"thursday\",\n          \"tuesday\",\n          \"wednesday\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n \
  \   }\n  },\n  \"required\": [\n    \"operation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-day-of-week-restriction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DayOfWeekRestriction
---
