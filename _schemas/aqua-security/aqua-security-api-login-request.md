---
description: LoginRequest schema from Aqua Security API
layout: schema
name: LoginRequest
properties_list:
- description: Username or user ID
  name: id
  type: string
- description: User password
  name: password
  type: string
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-login-request-schema.json
slug: aqua-security-api-login-request
source_filename: aqua-security-api-login-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"admin\",\n      \"description\": \"Username or user ID\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"example\": \"s3cur3P@ssw0rd\",\n      \"description\": \"User password\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"password\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-login-request-schema.json\",\n  \"title\": \"LoginRequest\",\n  \"description\": \"LoginRequest schema from Aqua Security API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-login-request-schema.json
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: LoginRequest
---
