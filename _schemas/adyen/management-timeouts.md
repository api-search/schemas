---
description: Timeouts schema from Adyen API
layout: schema
name: Timeouts
properties_list:
- description: Indicates the number of seconds of inactivity after which the terminal display goes into sleep mode.
  name: fromActiveToSleep
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-timeouts-schema.json
slug: management-timeouts
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-timeouts-schema.json\",\n  \"title\": \"Timeouts\",\n  \"description\": \"Timeouts schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fromActiveToSleep\": {\n      \"description\": \"Indicates the number of seconds of inactivity after which the terminal display goes into sleep mode.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-timeouts-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Timeouts
---
