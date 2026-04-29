---
description: TransactionBatch schema from Avalara API
layout: schema
name: TransactionBatch
properties_list:
- description: ''
  name: companyId
  type: string
- description: ''
  name: transactions
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/vat-reporting-transaction-batch-schema.json
slug: vat-reporting-transaction-batch
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/vat-reporting-transaction-batch-schema.json\",\n  \"title\": \"TransactionBatch\",\n  \"description\": \"TransactionBatch schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyId\": {\n      \"type\": \"string\"\n    },\n    \"transactions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/VATTransaction\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/vat-reporting-transaction-batch-schema.json
tags:
- Taxes
title: TransactionBatch
---
