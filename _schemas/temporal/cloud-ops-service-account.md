---
description: ''
layout: schema
name: ServiceAccount
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
provider_name: Temporal
provider_slug: temporal
schema_file: json-schema/cloud-ops-service-account-schema.json
slug: cloud-ops-service-account
source_filename: cloud-ops-service-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceAccount\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"resourceVersion\": {\n      \"type\": \"string\"\n    },\n    \"spec\": {\n      \"type\": \"object\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/json-schema/cloud-ops-service-account-schema.json
tags:
- ProCode_API_Composition
- Workflows
title: ServiceAccount
---
