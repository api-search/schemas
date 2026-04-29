---
description: Request body for adding a member to a group
layout: schema
name: GroupMemberAddRequest
properties_list:
- description: The ID of the user to add to the group
  name: userId
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-group-member-add-request-schema.json
slug: airbyte-group-member-add-request
source_filename: airbyte-group-member-add-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-group-member-add-request-schema.json\",\n  \"title\": \"GroupMemberAddRequest\",\n  \"description\": \"Request body for adding a member to a group\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The ID of the user to add to the group\"\n    }\n  },\n  \"required\": [\n    \"userId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-group-member-add-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: GroupMemberAddRequest
---
