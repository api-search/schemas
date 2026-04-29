---
description: It conveys the data to print and the way to process the print. It contains the complete content to print. Content of the Print Request message.
layout: schema
name: PrintRequest
properties_list:
- description: ''
  name: PrintOutput
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-print-request-schema.json
slug: terminal-print-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-print-request-schema.json\",\n  \"title\": \"PrintRequest\",\n  \"description\": \"It conveys the data to print and the way to process the print. It contains the complete content to print. Content of the Print Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PrintOutput\": {\n      \"$ref\": \"#/components/schemas/PrintOutput\"\n    }\n  },\n  \"required\": [\n    \"PrintOutput\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-print-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PrintRequest
---
