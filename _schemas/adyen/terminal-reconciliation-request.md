---
description: It conveys Information related to the Reconciliation requested by the Sale System. Content of the Reconciliation Request message.
layout: schema
name: ReconciliationRequest
properties_list:
- description: ''
  name: ReconciliationType
  type: object
- description: ''
  name: AcquirerID
  type: array
- description: Absent if ReconciliationType is not PreviousReconciliation.
  name: POIReconciliationID
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-reconciliation-request-schema.json
slug: terminal-reconciliation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-reconciliation-request-schema.json\",\n  \"title\": \"ReconciliationRequest\",\n  \"description\": \"It conveys Information related to the Reconciliation requested by the Sale System. Content of the Reconciliation Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReconciliationType\": {\n      \"$ref\": \"#/components/schemas/ReconciliationType\"\n    },\n    \"AcquirerID\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"description\": \"Could be present only if ReconciliationType is AcquirerReconciliation or AcquirerSynchronisation.\"\n      }\n    },\n    \"POIReconciliationID\": {\n      \"type\": \"integer\",\n      \"description\": \"Absent if ReconciliationType is not PreviousReconciliation.\"\n    }\n  },\n  \"required\": [\n  \
  \  \"ReconciliationType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-reconciliation-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ReconciliationRequest
---
