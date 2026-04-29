---
description: TimeOfDayRestriction schema from Adyen API
layout: schema
name: TimeOfDayRestriction
properties_list:
- description: Defines how the condition must be evaluated.
  name: operation
  type: string
- description: ''
  name: value
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-time-of-day-restriction-schema.json
slug: configuration-time-of-day-restriction
source_filename: configuration-time-of-day-restriction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-time-of-day-restriction-schema.json\",\n  \"title\": \"TimeOfDayRestriction\",\n  \"description\": \"TimeOfDayRestriction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"description\": \"Defines how the condition must be evaluated.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"$ref\": \"#/components/schemas/TimeOfDay\"\n    }\n  },\n  \"required\": [\n    \"operation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-time-of-day-restriction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TimeOfDayRestriction
---
