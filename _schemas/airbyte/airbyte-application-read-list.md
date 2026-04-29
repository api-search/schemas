---
description: ApplicationReadList schema from Airbyte API
layout: schema
name: ApplicationReadList
properties_list:
- description: ''
  name: applications
  type: array
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-application-read-list-schema.json
slug: airbyte-application-read-list
source_filename: airbyte-application-read-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-application-read-list-schema.json\",\n  \"title\": \"ApplicationReadList\",\n  \"description\": \"ApplicationReadList schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ApplicationRead\"\n      }\n    }\n  },\n  \"required\": [\n    \"applications\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-application-read-list-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: ApplicationReadList
---
