---
description: It conveys Information related to the Reconciliation transaction processed by the POI System. Content of the Reconciliation Response message.
layout: schema
name: GetTotalsResponse
properties_list:
- description: ''
  name: Response
  type: object
- description: Identification of the reconciliation period between Sale and POI.
  name: POIReconciliationID
  type: integer
- description: ''
  name: TransactionTotals
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-get-totals-response-schema.json
slug: terminal-get-totals-response
source_filename: terminal-get-totals-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-get-totals-response-schema.json\",\n  \"title\": \"GetTotalsResponse\",\n  \"description\": \"It conveys Information related to the Reconciliation transaction processed by the POI System. Content of the Reconciliation Response message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    },\n    \"POIReconciliationID\": {\n      \"type\": \"integer\",\n      \"description\": \"Identification of the reconciliation period between Sale and POI.\"\n    },\n    \"TransactionTotals\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransactionTotals\"\n      }\n    }\n  },\n  \"required\": [\n    \"Response\",\n    \"POIReconciliationID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-get-totals-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetTotalsResponse
---
