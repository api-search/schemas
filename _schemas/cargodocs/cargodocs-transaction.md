---
description: A transaction in the CargoDocs platform representing a trade or shipping workflow that groups related electronic documents together.
layout: schema
name: CargoDocs Transaction
properties_list:
- description: The unique identifier for the transaction.
  name: transactionId
  type: string
- description: The current status of the transaction.
  name: status
  type: string
- description: The timestamp when the transaction was created.
  name: createdAt
  type: string
- description: The number of documents associated with this transaction.
  name: documentCount
  type: integer
provider_name: CargoDocs
provider_slug: cargodocs
schema_file: json-schema/cargodocs-transaction.json
slug: cargodocs-transaction
source_filename: cargodocs-transaction.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/json-schema/cargodocs-transaction.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CargoDocs Transaction\",\n  \"description\": \"A transaction in the CargoDocs platform representing a trade or shipping workflow that groups related electronic documents together.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the transaction.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the transaction.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the transaction was created.\"\n    },\n    \"documentCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of documents associated with\
  \ this transaction.\"\n    }\n  },\n  \"required\": [\n    \"transactionId\",\n    \"status\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/json-schema/cargodocs-transaction.json
tags:
- Bills of Lading
- Documentation
- eBoL
- EssDocs
- MLETR
- Shipping
- Supply Chain
- Trade
- Trade Finance
- Warehouse Warrants
title: CargoDocs Transaction
---
