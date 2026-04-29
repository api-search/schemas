---
description: Duration schema from Adyen API
layout: schema
name: Duration
properties_list:
- description: 'The unit of time. You can only use **minutes** and **hours** if the `interval.type` is **sliding**. Possible values: **minutes**, **hours**, **days**, **weeks**, or **months**'
  name: unit
  type: string
- description: The length of time by the unit. For example, 5 days. The maximum duration is 90 days or an equivalent in other units. For example, 3 months.
  name: value
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-duration-schema.json
slug: configuration-duration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-duration-schema.json\",\n  \"title\": \"Duration\",\n  \"description\": \"Duration schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"unit\": {\n      \"description\": \"The unit of time. You can only use **minutes** and **hours** if the `interval.type` is **sliding**.\\n\\nPossible values: **minutes**, **hours**, **days**, **weeks**, or **months**\",\n      \"enum\": [\n        \"days\",\n        \"hours\",\n        \"minutes\",\n        \"months\",\n        \"weeks\"\n      ],\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The length of time by the unit. For example, 5 days.\\n\\nThe maximum duration is 90 days or an equivalent in other units. For example, 3 months.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n \
  \ }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-duration-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Duration
---
