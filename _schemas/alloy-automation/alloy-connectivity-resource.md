---
description: A resource entity available in a connector
layout: schema
name: Resource
properties_list:
- description: Unique identifier for the resource
  name: resourceId
  type: string
- description: Display name of the resource
  name: name
  type: string
- description: Description of the resource
  name: description
  type: string
- description: List of supported action names for this resource
  name: actions
  type: array
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-resource-schema.json
slug: alloy-connectivity-resource
source_filename: alloy-connectivity-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-resource-schema.json\",\n  \"title\": \"Resource\",\n  \"type\": \"object\",\n  \"description\": \"A resource entity available in a connector\",\n  \"properties\": {\n    \"resourceId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the resource\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the resource\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the resource\"\n    },\n    \"actions\": {\n      \"type\": \"array\",\n      \"description\": \"List of supported action names for this resource\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-resource-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: Resource
---
