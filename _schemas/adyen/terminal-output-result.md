---
description: In the message response, it contains the result of the output, if required in the message request. Information related to the result the output (display, print, input).
layout: schema
name: OutputResult
properties_list:
- description: ''
  name: Device
  type: object
- description: ''
  name: InfoQualify
  type: object
- description: ''
  name: Response
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-output-result-schema.json
slug: terminal-output-result
source_filename: terminal-output-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-output-result-schema.json\",\n  \"title\": \"OutputResult\",\n  \"description\": \"In the message response, it contains the result of the output, if required in the message request. Information related to the result the output (display, print, input).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Device\": {\n      \"$ref\": \"#/components/schemas/Device\"\n    },\n    \"InfoQualify\": {\n      \"$ref\": \"#/components/schemas/InfoQualify\"\n    },\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    }\n  },\n  \"required\": [\n    \"Device\",\n    \"InfoQualify\",\n    \"Response\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-output-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: OutputResult
---
