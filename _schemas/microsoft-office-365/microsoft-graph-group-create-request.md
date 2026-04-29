---
description: ''
layout: schema
name: GroupCreateRequest
properties_list:
- description: The display name for the group.
  name: displayName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: mailEnabled
  type: boolean
- description: ''
  name: mailNickname
  type: string
- description: ''
  name: securityEnabled
  type: boolean
- description: Set to ["Unified"] to create a Microsoft 365 group.
  name: groupTypes
  type: array
- description: ''
  name: visibility
  type: string
- description: URLs of user objects to set as owners at creation time.
  name: owners@odata.bind
  type: array
- description: URLs of user objects to set as members at creation time.
  name: members@odata.bind
  type: array
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-group-create-request-schema.json
slug: microsoft-graph-group-create-request
source_filename: microsoft-graph-group-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name for the group.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"mailEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"mailNickname\": {\n      \"type\": \"string\"\n    },\n    \"securityEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"groupTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Set to [\\\"Unified\\\"] to create a Microsoft 365 group.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\"\n    },\n    \"owners@odata.bind\": {\n      \"type\": \"array\",\n      \"description\": \"URLs of user objects to set as owners at creation time.\"\n    },\n    \"members@odata.bind\": {\n      \"type\": \"array\",\n      \"description\": \"URLs of user objects to set as\
  \ members at creation time.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-group-create-request-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: GroupCreateRequest
---
