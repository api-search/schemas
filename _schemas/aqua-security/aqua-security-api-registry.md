---
description: Registry schema from Aqua Security API
layout: schema
name: Registry
properties_list:
- description: Registry display name
  name: name
  type: string
- description: Registry type
  name: type
  type: string
- description: Registry URL
  name: url
  type: string
- description: Authentication username
  name: username
  type: string
- description: Connection status
  name: status
  type: string
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-registry-schema.json
slug: aqua-security-api-registry
source_filename: aqua-security-api-registry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"docker-hub\",\n      \"description\": \"Registry display name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"HUB\",\n        \"V2\",\n        \"ECR\",\n        \"ACR\",\n        \"GCR\",\n        \"JFrog\",\n        \"Harbor\"\n      ],\n      \"example\": \"HUB\",\n      \"description\": \"Registry type\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://index.docker.io\",\n      \"description\": \"Registry URL\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"example\": \"myuser\",\n      \"description\": \"Authentication username\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"connected\",\n        \"disconnected\",\n        \"error\"\n      ],\n      \"example\": \"connected\",\n      \"description\": \"Connection status\"\n  \
  \  }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-registry-schema.json\",\n  \"title\": \"Registry\",\n  \"description\": \"Registry schema from Aqua Security API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-registry-schema.json
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: Registry
---
