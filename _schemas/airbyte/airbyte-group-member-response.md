---
description: Provides details of a single group member
layout: schema
name: GroupMemberResponse
properties_list:
- description: The ID of the group membership
  name: memberId
  type: string
- description: The ID of the group
  name: groupId
  type: string
- description: The ID of the user
  name: userId
  type: string
- description: The email of the user
  name: userEmail
  type: string
- description: The name of the user
  name: userName
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-group-member-response-schema.json
slug: airbyte-group-member-response
source_filename: airbyte-group-member-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-group-member-response-schema.json\",\n  \"title\": \"GroupMemberResponse\",\n  \"description\": \"Provides details of a single group member\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"memberId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The ID of the group membership\"\n    },\n    \"groupId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The ID of the group\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The ID of the user\"\n    },\n    \"userEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email of the user\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The name of the user\"\n    }\n  },\n  \"required\": [\n    \"memberId\",\n    \"groupId\",\n    \"userId\",\n    \"userEmail\",\n    \"userName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-group-member-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: GroupMemberResponse
---
