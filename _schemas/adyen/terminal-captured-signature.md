---
description: CapturedSignature schema from Adyen API
layout: schema
name: CapturedSignature
properties_list:
- description: ''
  name: AreaSize
  type: object
- description: ''
  name: SignaturePoint
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-captured-signature-schema.json
slug: terminal-captured-signature
source_filename: terminal-captured-signature-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-captured-signature-schema.json\",\n  \"title\": \"CapturedSignature\",\n  \"description\": \"CapturedSignature schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AreaSize\": {\n      \"$ref\": \"#/components/schemas/AreaSize\"\n    },\n    \"SignaturePoint\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Point\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-captured-signature-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CapturedSignature
---
