---
description: LoginResponse schema from Aqua Security API
layout: schema
name: LoginResponse
properties_list:
- description: JWT bearer token for subsequent API calls
  name: token
  type: string
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-login-response-schema.json
slug: aqua-security-api-login-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"example\": \"eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.abc123\",\n      \"description\": \"JWT bearer token for subsequent API calls\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-login-response-schema.json\",\n  \"title\": \"LoginResponse\",\n  \"description\": \"LoginResponse schema from Aqua Security API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-login-response-schema.json
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: LoginResponse
---
