---
description: ''
layout: schema
name: VersionDefinition
properties_list:
- description: ''
  name: default
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: fallback_to_default
  type: boolean
- description: ''
  name: key
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: strip_path
  type: boolean
- description: ''
  name: strip_versioning_data
  type: boolean
- description: ''
  name: url_versioning_pattern
  type: string
- description: ''
  name: versions
  type: object
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-version-definition-schema.json
slug: tyk-gateway-version-definition
source_filename: tyk-gateway-version-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VersionDefinition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"default\": {\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"fallback_to_default\": {\n      \"type\": \"boolean\"\n    },\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"strip_path\": {\n      \"type\": \"boolean\"\n    },\n    \"strip_versioning_data\": {\n      \"type\": \"boolean\"\n    },\n    \"url_versioning_pattern\": {\n      \"type\": \"string\"\n    },\n    \"versions\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-version-definition-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: VersionDefinition
---
