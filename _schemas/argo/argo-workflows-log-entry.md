---
description: LogEntry schema from Argo API
layout: schema
name: LogEntry
properties_list:
- description: ''
  name: content
  type: string
- description: ''
  name: podName
  type: string
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-log-entry-schema.json
slug: argo-workflows-log-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-log-entry-schema.json\",\n  \"title\": \"LogEntry\",\n  \"description\": \"LogEntry schema from Argo API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"string\"\n    },\n    \"podName\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-log-entry-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: LogEntry
---
