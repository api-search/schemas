---
description: Hardware schema from Adyen API
layout: schema
name: Hardware
properties_list:
- description: The brightness of the display when the terminal is being used, expressed as a percentage.
  name: displayMaximumBackLight
  type: integer
- description: 'The hour of the day when the terminal is set to reset the Totals report. By default, the reset hour is at 6:00 AM in the timezone of the terminal. Minimum value: 0, maximum value: 23.'
  name: resetTotalsHour
  type: integer
- description: 'The hour of the day when the terminal is set to reboot to apply the configuration and software updates. By default, the restart hour is at 6:00 AM in the timezone of the terminal. Minimum value: 0, ma'
  name: restartHour
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-hardware-schema.json
slug: management-hardware
source_filename: management-hardware-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-hardware-schema.json\",\n  \"title\": \"Hardware\",\n  \"description\": \"Hardware schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayMaximumBackLight\": {\n      \"description\": \"The brightness of the display when the terminal is being used, expressed as a percentage.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"resetTotalsHour\": {\n      \"description\": \"The hour of the day when the terminal is set to reset the Totals report. By default, the reset hour is at 6:00 AM in the timezone of the terminal. Minimum value: 0, maximum value: 23.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"restartHour\": {\n      \"description\": \"The hour of the day when the terminal is set to reboot to apply the configuration\
  \ and software updates. By default, the restart hour is at 6:00 AM in the timezone of the terminal. Minimum value: 0, maximum value: 23.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-hardware-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Hardware
---
