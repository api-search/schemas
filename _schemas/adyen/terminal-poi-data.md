---
description: In the Message Response, identification of the POI transaction. Data related to the POI System.
layout: schema
name: POIData
properties_list:
- description: ''
  name: POITransactionID
  type: object
- description: If Result is Success.
  name: POIReconciliationID
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-poi-data-schema.json
slug: terminal-poi-data
source_filename: terminal-poi-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-poi-data-schema.json\",\n  \"title\": \"POIData\",\n  \"description\": \"In the Message Response, identification of the POI transaction. Data related to the POI System.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"POITransactionID\": {\n      \"$ref\": \"#/components/schemas/TransactionIDType\"\n    },\n    \"POIReconciliationID\": {\n      \"type\": \"integer\",\n      \"description\": \"If Result is Success.\"\n    }\n  },\n  \"required\": [\n    \"POITransactionID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-poi-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: POIData
---
