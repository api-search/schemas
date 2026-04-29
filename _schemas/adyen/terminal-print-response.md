---
description: It conveys the result of the print, parallel to the message request, except if response not required and absent. Content of the Print Response message.
layout: schema
name: PrintResponse
properties_list:
- description: ''
  name: DocumentQualifier
  type: object
- description: ''
  name: Response
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-print-response-schema.json
slug: terminal-print-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-print-response-schema.json\",\n  \"title\": \"PrintResponse\",\n  \"description\": \"It conveys the result of the print, parallel to the message request, except if response not required and absent. Content of the Print Response message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DocumentQualifier\": {\n      \"$ref\": \"#/components/schemas/DocumentQualifier\"\n    },\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    }\n  },\n  \"required\": [\n    \"DocumentQualifier\",\n    \"Response\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-print-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PrintResponse
---
