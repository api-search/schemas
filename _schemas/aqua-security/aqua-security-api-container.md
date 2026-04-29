---
description: Container schema from Aqua Security API
layout: schema
name: Container
properties_list:
- description: Container ID
  name: container_id
  type: string
- description: Container name
  name: name
  type: string
- description: Image name and tag
  name: image
  type: string
- description: Container runtime status
  name: status
  type: string
- description: Applied security policy name
  name: policy
  type: string
- description: Host running the container
  name: host
  type: string
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-container-schema.json
slug: aqua-security-api-container
source_filename: aqua-security-api-container-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"container_id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123def456\",\n      \"description\": \"Container ID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"web-server-1\",\n      \"description\": \"Container name\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"example\": \"nginx:latest\",\n      \"description\": \"Image name and tag\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"running\",\n        \"stopped\",\n        \"paused\"\n      ],\n      \"example\": \"running\",\n      \"description\": \"Container runtime status\"\n    },\n    \"policy\": {\n      \"type\": \"string\",\n      \"example\": \"default\",\n      \"description\": \"Applied security policy name\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"example\": \"kube-node-01\",\n      \"description\": \"Host running the container\"\n  \
  \  }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-container-schema.json\",\n  \"title\": \"Container\",\n  \"description\": \"Container schema from Aqua Security API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-container-schema.json
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: Container
---
