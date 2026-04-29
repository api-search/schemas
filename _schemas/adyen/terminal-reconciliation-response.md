---
description: It conveys Information related to the Reconciliation transaction processed by the POI System. Content of the Reconciliation Response message.
layout: schema
name: ReconciliationResponse
properties_list:
- description: ''
  name: Response
  type: object
- description: ''
  name: ReconciliationType
  type: object
- description: Absent if ReconciliationType is AcquirerReconciliation.
  name: POIReconciliationID
  type: integer
- description: ''
  name: TransactionTotals
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-reconciliation-response-schema.json
slug: terminal-reconciliation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-reconciliation-response-schema.json\",\n  \"title\": \"ReconciliationResponse\",\n  \"description\": \"It conveys Information related to the Reconciliation transaction processed by the POI System. Content of the Reconciliation Response message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    },\n    \"ReconciliationType\": {\n      \"$ref\": \"#/components/schemas/ReconciliationType\"\n    },\n    \"POIReconciliationID\": {\n      \"type\": \"integer\",\n      \"description\": \"Absent if ReconciliationType is AcquirerReconciliation.\"\n    },\n    \"TransactionTotals\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransactionTotals\"\n      }\n    }\n  },\n  \"required\": [\n   \
  \ \"Response\",\n    \"ReconciliationType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-reconciliation-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ReconciliationResponse
---
