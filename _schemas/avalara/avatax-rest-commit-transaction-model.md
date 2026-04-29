---
description: CommitTransactionModel schema from Avalara API
layout: schema
name: CommitTransactionModel
properties_list:
- description: Set to true to commit the transaction
  name: commit
  type: boolean
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-commit-transaction-model-schema.json
slug: avatax-rest-commit-transaction-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-commit-transaction-model-schema.json\",\n  \"title\": \"CommitTransactionModel\",\n  \"description\": \"CommitTransactionModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"commit\"\n  ],\n  \"properties\": {\n    \"commit\": {\n      \"type\": \"boolean\",\n      \"description\": \"Set to true to commit the transaction\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-commit-transaction-model-schema.json
tags:
- Taxes
title: CommitTransactionModel
---
