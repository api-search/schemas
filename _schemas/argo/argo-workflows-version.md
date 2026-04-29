---
description: Version schema from Argo API
layout: schema
name: Version
properties_list:
- description: ''
  name: version
  type: string
- description: ''
  name: buildDate
  type: string
- description: ''
  name: gitCommit
  type: string
- description: ''
  name: gitTag
  type: string
- description: ''
  name: gitTreeState
  type: string
- description: ''
  name: goVersion
  type: string
- description: ''
  name: compiler
  type: string
- description: ''
  name: platform
  type: string
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-version-schema.json
slug: argo-workflows-version
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-version-schema.json\",\n  \"title\": \"Version\",\n  \"description\": \"Version schema from Argo API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\"\n    },\n    \"buildDate\": {\n      \"type\": \"string\"\n    },\n    \"gitCommit\": {\n      \"type\": \"string\"\n    },\n    \"gitTag\": {\n      \"type\": \"string\"\n    },\n    \"gitTreeState\": {\n      \"type\": \"string\"\n    },\n    \"goVersion\": {\n      \"type\": \"string\"\n    },\n    \"compiler\": {\n      \"type\": \"string\"\n    },\n    \"platform\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-version-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Version
---
