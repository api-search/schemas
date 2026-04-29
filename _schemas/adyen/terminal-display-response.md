---
description: It conveys the result of the display, parallel to the message request, except if response not required and absent. Content of the Display Response message.
layout: schema
name: DisplayResponse
properties_list:
- description: ''
  name: OutputResult
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-display-response-schema.json
slug: terminal-display-response
source_filename: terminal-display-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-display-response-schema.json\",\n  \"title\": \"DisplayResponse\",\n  \"description\": \"It conveys the result of the display, parallel to the message request, except if response not required and absent. Content of the Display Response message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutputResult\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/OutputResult\"\n      }\n    }\n  },\n  \"required\": [\n    \"OutputResult\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-display-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DisplayResponse
---
