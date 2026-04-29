---
description: Path to a field/column/property in a stream to be selected. For example, if the field to be selected is a database column called "foo", this will be ["foo"]. Use multiple path elements for nested schemas.
layout: schema
name: SelectedFieldInfo
properties_list:
- description: ''
  name: fieldPath
  type: array
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-selected-field-info-schema.json
slug: airbyte-selected-field-info
source_filename: airbyte-selected-field-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-selected-field-info-schema.json\",\n  \"title\": \"SelectedFieldInfo\",\n  \"description\": \"Path to a field/column/property in a stream to be selected. For example, if the field to be selected is a database column called \\\"foo\\\", this will be [\\\"foo\\\"]. Use multiple path elements for nested schemas.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldPath\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-selected-field-info-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: SelectedFieldInfo
---
