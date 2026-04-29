---
description: Error response from the API
layout: schema
name: Error
properties_list:
- description: Human-readable error message
  name: error
  type: string
provider_name: 42Crunch
provider_slug: 42crunch
schema_file: json-schema/scand-manager-error-schema.json
slug: scand-manager-error
source_filename: scand-manager-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/42crunch/refs/heads/main/json-schema/scand-manager-error-schema.json\",\n  \"title\": \"Error\",\n  \"description\": \"Error response from the API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\",\n      \"maxLength\": 1024,\n      \"minLength\": 1,\n      \"pattern\": \"^\\\\P{Cc}+$\",\n      \"example\": \"Job not found\"\n    }\n  },\n  \"additionalProperties\": false,\n  \"required\": [\n    \"error\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/42crunch/refs/heads/main/json-schema/scand-manager-error-schema.json
tags:
- API Security
- Platform
- Scanning
- Security
- OpenAPI
- DevSecOps
title: Error
---
