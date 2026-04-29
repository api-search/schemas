---
description: RegistryList schema from Aqua Security API
layout: schema
name: RegistryList
properties_list:
- description: Total number of registries
  name: count
  type: integer
- description: ''
  name: result
  type: array
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-registry-list-schema.json
slug: aqua-security-api-registry-list
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"example\": 3,\n      \"description\": \"Total number of registries\"\n    },\n    \"result\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"docker-hub\",\n            \"description\": \"Registry display name\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"HUB\",\n              \"V2\",\n              \"ECR\",\n              \"ACR\",\n              \"GCR\",\n              \"JFrog\",\n              \"Harbor\"\n            ],\n            \"example\": \"HUB\",\n            \"description\": \"Registry type\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://index.docker.io\",\n            \"description\": \"\
  Registry URL\"\n          },\n          \"username\": {\n            \"type\": \"string\",\n            \"example\": \"myuser\",\n            \"description\": \"Authentication username\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"connected\",\n              \"disconnected\",\n              \"error\"\n            ],\n            \"example\": \"connected\",\n            \"description\": \"Connection status\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-registry-list-schema.json\",\n  \"title\": \"RegistryList\",\n  \"description\": \"RegistryList schema from Aqua Security API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-registry-list-schema.json
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: RegistryList
---
