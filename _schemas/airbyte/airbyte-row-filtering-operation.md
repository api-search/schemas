---
description: RowFilteringOperation schema from Airbyte API
layout: schema
name: RowFilteringOperation
properties_list: []
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-row-filtering-operation-schema.json
slug: airbyte-row-filtering-operation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-row-filtering-operation-schema.json\",\n  \"title\": \"RowFilteringOperation\",\n  \"description\": \"RowFilteringOperation schema from Airbyte API\",\n  \"type\": \"object\",\n  \"oneOf\": [\n    {\n      \"$ref\": \"#/components/schemas/RowFilteringOperationEqual\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/RowFilteringOperationNot\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-row-filtering-operation-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: RowFilteringOperation
---
