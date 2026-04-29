---
description: ''
layout: schema
name: VersionData
properties_list:
- description: ''
  name: default_version
  type: string
- description: ''
  name: not_versioned
  type: boolean
- description: ''
  name: versions
  type: object
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-version-data-schema.json
slug: tyk-gateway-version-data
source_filename: tyk-gateway-version-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VersionData\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"default_version\": {\n      \"type\": \"string\"\n    },\n    \"not_versioned\": {\n      \"type\": \"boolean\"\n    },\n    \"versions\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-version-data-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: VersionData
---
