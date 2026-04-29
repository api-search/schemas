---
description: It conveys the data to display and the way to process the display. It contains the complete content to display. It might contain an operation (the DisplayOutput element) per Display Device type. Content of the Display Request message.
layout: schema
name: DisplayRequest
properties_list:
- description: ''
  name: DisplayOutput
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-display-request-schema.json
slug: terminal-display-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-display-request-schema.json\",\n  \"title\": \"DisplayRequest\",\n  \"description\": \"It conveys the data to display and the way to process the display. It contains the complete content to display. It might contain an operation (the DisplayOutput element) per Display Device type. Content of the Display Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DisplayOutput\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DisplayOutput\"\n      }\n    }\n  },\n  \"required\": [\n    \"DisplayOutput\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-display-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DisplayRequest
---
