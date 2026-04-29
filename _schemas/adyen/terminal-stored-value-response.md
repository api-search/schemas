---
description: It conveys Information related to the Stored Value transaction processed by the POI System. Content of the Stored Value Response message.
layout: schema
name: StoredValueResponse
properties_list:
- description: ''
  name: Response
  type: object
- description: ''
  name: SaleData
  type: object
- description: ''
  name: POIData
  type: object
- description: ''
  name: StoredValueResult
  type: array
- description: ''
  name: PaymentReceipt
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-stored-value-response-schema.json
slug: terminal-stored-value-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-stored-value-response-schema.json\",\n  \"title\": \"StoredValueResponse\",\n  \"description\": \"It conveys Information related to the Stored Value transaction processed by the POI System. Content of the Stored Value Response message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    },\n    \"SaleData\": {\n      \"$ref\": \"#/components/schemas/SaleData\"\n    },\n    \"POIData\": {\n      \"$ref\": \"#/components/schemas/POIData\"\n    },\n    \"StoredValueResult\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StoredValueResult\"\n      }\n    },\n    \"PaymentReceipt\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PaymentReceipt\"\n\
  \      }\n    }\n  },\n  \"required\": [\n    \"Response\",\n    \"SaleData\",\n    \"POIData\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-stored-value-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoredValueResponse
---
