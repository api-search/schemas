---
description: VoidTransactionModel schema from Avalara API
layout: schema
name: VoidTransactionModel
properties_list:
- description: Reason for voiding the transaction
  name: code
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-void-transaction-model-schema.json
slug: avatax-rest-void-transaction-model
source_filename: avatax-rest-void-transaction-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-void-transaction-model-schema.json\",\n  \"title\": \"VoidTransactionModel\",\n  \"description\": \"VoidTransactionModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"code\"\n  ],\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Unspecified\",\n        \"PostFailed\",\n        \"DocDeleted\",\n        \"DocVoided\",\n        \"AdjustmentCancelled\"\n      ],\n      \"description\": \"Reason for voiding the transaction\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-void-transaction-model-schema.json
tags:
- Taxes
title: VoidTransactionModel
---
