---
description: It conveys Information related to the Stored Value transaction to process. Content of the Stored Value Request message.
layout: schema
name: StoredValueRequest
properties_list:
- description: ''
  name: SaleData
  type: object
- description: If the language is selected by the Sale System before the request to the POI.
  name: CustomerLanguage
  type: string
- description: ''
  name: StoredValueData
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-stored-value-request-schema.json
slug: terminal-stored-value-request
source_filename: terminal-stored-value-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-stored-value-request-schema.json\",\n  \"title\": \"StoredValueRequest\",\n  \"description\": \"It conveys Information related to the Stored Value transaction to process. Content of the Stored Value Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SaleData\": {\n      \"$ref\": \"#/components/schemas/SaleData\"\n    },\n    \"CustomerLanguage\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[a-z]{2,2}$\",\n      \"description\": \"If the language is selected by the Sale System before the request to the POI.\"\n    },\n    \"StoredValueData\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StoredValueData\"\n      }\n    }\n  },\n  \"required\": [\n    \"SaleData\",\n    \"StoredValueData\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-stored-value-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoredValueRequest
---
