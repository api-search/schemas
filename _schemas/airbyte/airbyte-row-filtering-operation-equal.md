---
description: RowFilteringOperationEqual schema from Airbyte API
layout: schema
name: RowFilteringOperationEqual
properties_list:
- description: The value to compare the field against.
  name: comparisonValue
  type: string
- description: The name of the field to apply the operation on.
  name: fieldName
  type: string
- description: ''
  name: type
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-row-filtering-operation-equal-schema.json
slug: airbyte-row-filtering-operation-equal
source_filename: airbyte-row-filtering-operation-equal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-row-filtering-operation-equal-schema.json\",\n  \"title\": \"RowFilteringOperationEqual\",\n  \"description\": \"RowFilteringOperationEqual schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"comparisonValue\": {\n      \"type\": \"string\",\n      \"title\": \"Comparison Value\",\n      \"description\": \"The value to compare the field against.\"\n    },\n    \"fieldName\": {\n      \"type\": \"string\",\n      \"title\": \"Field Name\",\n      \"description\": \"The name of the field to apply the operation on.\"\n    },\n    \"type\": {\n      \"$ref\": \"#/components/schemas/RowFilteringOperationType\"\n    }\n  },\n  \"required\": [\n    \"comparisonValue\",\n    \"fieldName\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-row-filtering-operation-equal-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: RowFilteringOperationEqual
---
