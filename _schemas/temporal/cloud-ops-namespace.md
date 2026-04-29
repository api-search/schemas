---
description: ''
layout: schema
name: Namespace
properties_list:
- description: ''
  name: namespace
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
  name: asyncOperationId
  type: string
- description: ''
  name: endpoints
  type: object
- description: ''
  name: createdTime
  type: string
- description: ''
  name: lastModifiedTime
  type: string
provider_name: Temporal
provider_slug: temporal
schema_file: json-schema/cloud-ops-namespace-schema.json
slug: cloud-ops-namespace
source_filename: cloud-ops-namespace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Namespace\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"resourceVersion\": {\n      \"type\": \"string\"\n    },\n    \"spec\": {\n      \"type\": \"object\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"asyncOperationId\": {\n      \"type\": \"string\"\n    },\n    \"endpoints\": {\n      \"type\": \"object\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\"\n    },\n    \"lastModifiedTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/json-schema/cloud-ops-namespace-schema.json
tags:
- ProCode_API_Composition
- Workflows
title: Namespace
---
