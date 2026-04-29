---
description: Provides details of a single group
layout: schema
name: GroupResponse
properties_list:
- description: The ID of the group
  name: groupId
  type: string
- description: The name of the group
  name: name
  type: string
- description: Optional description of the group
  name: description
  type: string
- description: The ID of the organization the group belongs to
  name: organizationId
  type: string
- description: The number of members in the group
  name: memberCount
  type: integer
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-group-response-schema.json
slug: airbyte-group-response
source_filename: airbyte-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-group-response-schema.json\",\n  \"title\": \"GroupResponse\",\n  \"description\": \"Provides details of a single group\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groupId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The ID of the group\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the group\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Optional description of the group\"\n    },\n    \"organizationId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The ID of the organization the group belongs to\"\n    },\n    \"memberCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n \
  \     \"description\": \"The number of members in the group\"\n    }\n  },\n  \"required\": [\n    \"groupId\",\n    \"name\",\n    \"organizationId\",\n    \"memberCount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-group-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: GroupResponse
---
