---
description: RowFilteringOperationNot schema from Airbyte API
layout: schema
name: RowFilteringOperationNot
properties_list:
- description: Conditions to evaluate with the NOT operator.
  name: conditions
  type: array
- description: ''
  name: type
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-row-filtering-operation-not-schema.json
slug: airbyte-row-filtering-operation-not
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-row-filtering-operation-not-schema.json\",\n  \"title\": \"RowFilteringOperationNot\",\n  \"description\": \"RowFilteringOperationNot schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"conditions\": {\n      \"title\": \"Sub-Conditions (NOT)\",\n      \"description\": \"Conditions to evaluate with the NOT operator.\",\n      \"minItems\": 1,\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RowFilteringOperation\"\n      }\n    },\n    \"type\": {\n      \"$ref\": \"#/components/schemas/RowFilteringOperationType\"\n    }\n  },\n  \"required\": [\n    \"conditions\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-row-filtering-operation-not-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: RowFilteringOperationNot
---
