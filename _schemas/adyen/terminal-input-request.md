---
description: It conveys data to display and the way to process the display, and contains the complete content to display. In addition to the display on the Input Device, it might contain an operation (the DisplayOutput element) per Display Device type. Content of the Input Request message.
layout: schema
name: InputRequest
properties_list:
- description: ''
  name: DisplayOutput
  type: object
- description: ''
  name: InputData
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-input-request-schema.json
slug: terminal-input-request
source_filename: terminal-input-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-input-request-schema.json\",\n  \"title\": \"InputRequest\",\n  \"description\": \"It conveys data to display and the way to process the display, and contains the complete content to display. In addition to the display on the Input Device, it might contain an operation (the DisplayOutput element) per Display Device type. Content of the Input Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DisplayOutput\": {\n      \"$ref\": \"#/components/schemas/DisplayOutput\"\n    },\n    \"InputData\": {\n      \"$ref\": \"#/components/schemas/InputData\"\n    }\n  },\n  \"required\": [\n    \"InputData\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-input-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: InputRequest
---
