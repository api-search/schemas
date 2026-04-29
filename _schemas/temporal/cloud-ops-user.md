---
description: ''
layout: schema
name: User
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: resourceVersion
  type: string
- description: ''
  name: spec
  type: object
- description: ''
  name: state
  type: string
- description: ''
  name: createdTime
  type: string
- description: ''
  name: lastModifiedTime
  type: string
provider_name: Temporal
provider_slug: temporal
schema_file: json-schema/cloud-ops-user-schema.json
slug: cloud-ops-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"resourceVersion\": {\n      \"type\": \"string\"\n    },\n    \"spec\": {\n      \"type\": \"object\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\"\n    },\n    \"lastModifiedTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/json-schema/cloud-ops-user-schema.json
tags:
- ProCode_API_Composition
- Workflows
title: User
---
