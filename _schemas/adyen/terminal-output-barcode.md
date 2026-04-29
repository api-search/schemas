---
description: OutputBarcode schema from Adyen API
layout: schema
name: OutputBarcode
properties_list:
- description: ''
  name: BarcodeType
  type: object
- description: ''
  name: BarcodeValue
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-output-barcode-schema.json
slug: terminal-output-barcode
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-output-barcode-schema.json\",\n  \"title\": \"OutputBarcode\",\n  \"description\": \"OutputBarcode schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BarcodeType\": {\n      \"$ref\": \"#/components/schemas/BarcodeType\"\n    },\n    \"BarcodeValue\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    }\n  },\n  \"required\": [\n    \"BarcodeValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-output-barcode-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: OutputBarcode
---
