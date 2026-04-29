---
description: Paths to the fields that will be included in the configured catalog.
layout: schema
name: SelectedFields
properties_list: []
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-selected-fields-schema.json
slug: airbyte-selected-fields
source_filename: airbyte-selected-fields-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-selected-fields-schema.json\",\n  \"title\": \"SelectedFields\",\n  \"description\": \"Paths to the fields that will be included in the configured catalog.\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/SelectedFieldInfo\"\n  },\n  \"format\": \"set\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-selected-fields-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: SelectedFields
---
