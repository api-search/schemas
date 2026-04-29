---
description: It conveys the result of the input or the result of the outputs, parallel to the message request, except if response not required and absent. Content of the Input Response message.
layout: schema
name: InputResponse
properties_list:
- description: ''
  name: OutputResult
  type: object
- description: ''
  name: InputResult
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-input-response-schema.json
slug: terminal-input-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-input-response-schema.json\",\n  \"title\": \"InputResponse\",\n  \"description\": \"It conveys the result of the input or the result of the outputs, parallel to the message request, except if response not required and absent. Content of the Input Response message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutputResult\": {\n      \"$ref\": \"#/components/schemas/OutputResult\"\n    },\n    \"InputResult\": {\n      \"$ref\": \"#/components/schemas/InputResult\"\n    }\n  },\n  \"required\": [\n    \"InputResult\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-input-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: InputResponse
---
