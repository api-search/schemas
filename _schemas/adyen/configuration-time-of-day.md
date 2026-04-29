---
description: TimeOfDay schema from Adyen API
layout: schema
name: TimeOfDay
properties_list:
- description: 'The end time in a time-only ISO-8601 extended offset format. For example: **08:00:00+02:00**, **22:30:00-03:00**.'
  name: endTime
  type: string
- description: 'The start time in a time-only ISO-8601 extended offset format. For example: **08:00:00+02:00**, **22:30:00-03:00**.'
  name: startTime
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-time-of-day-schema.json
slug: configuration-time-of-day
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-time-of-day-schema.json\",\n  \"title\": \"TimeOfDay\",\n  \"description\": \"TimeOfDay schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endTime\": {\n      \"description\": \"The end time in a time-only ISO-8601 extended offset format. For example: **08:00:00+02:00**, **22:30:00-03:00**.\\n\\n\",\n      \"type\": \"string\"\n    },\n    \"startTime\": {\n      \"description\": \"The start time in a time-only ISO-8601 extended offset format. For example: **08:00:00+02:00**, **22:30:00-03:00**.\\n\\n\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-time-of-day-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TimeOfDay
---
