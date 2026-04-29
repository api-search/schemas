---
description: InputResult schema from Adyen API
layout: schema
name: InputResult
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
- description: ''
  name: Input
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-input-result-schema.json
slug: terminal-input-result
source_filename: terminal-input-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-input-result-schema.json\",\n  \"title\": \"InputResult\",\n  \"description\": \"InputResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Device\": {\n      \"$ref\": \"#/components/schemas/Device\"\n    },\n    \"InfoQualify\": {\n      \"$ref\": \"#/components/schemas/InfoQualify\"\n    },\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    },\n    \"Input\": {\n      \"$ref\": \"#/components/schemas/Input\"\n    }\n  },\n  \"required\": [\n    \"Device\",\n    \"InfoQualify\",\n    \"Response\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-input-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: InputResult
---
