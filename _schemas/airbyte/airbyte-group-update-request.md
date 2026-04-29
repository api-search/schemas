---
description: Request body for updating a group
layout: schema
name: GroupUpdateRequest
properties_list:
- description: The updated name of the group
  name: name
  type: string
- description: The updated description of the group
  name: description
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-group-update-request-schema.json
slug: airbyte-group-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-group-update-request-schema.json\",\n  \"title\": \"GroupUpdateRequest\",\n  \"description\": \"Request body for updating a group\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The updated name of the group\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"The updated description of the group\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-group-update-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: GroupUpdateRequest
---
