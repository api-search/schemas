---
description: ErrorResponse schema from Aqua Security API
layout: schema
name: ErrorResponse
properties_list:
- description: Human-readable error description
  name: message
  type: string
- description: Error code
  name: code
  type: integer
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-error-response-schema.json
slug: aqua-security-api-error-response
source_filename: aqua-security-api-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"Unauthorized access\",\n      \"description\": \"Human-readable error description\"\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"example\": 401,\n      \"description\": \"Error code\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-error-response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"ErrorResponse schema from Aqua Security API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-error-response-schema.json
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: ErrorResponse
---
