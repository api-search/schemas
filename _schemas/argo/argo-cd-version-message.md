---
description: Argo CD server version information.
layout: schema
name: VersionMessage
properties_list:
- description: Argo CD version string.
  name: Version
  type: string
- description: Build date.
  name: BuildDate
  type: string
- description: Git commit SHA of this build.
  name: GitCommit
  type: string
- description: Go language version used to build.
  name: GoVersion
  type: string
- description: Operating system and architecture.
  name: Platform
  type: string
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-version-message-schema.json
slug: argo-cd-version-message
source_filename: argo-cd-version-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-version-message-schema.json\",\n  \"title\": \"VersionMessage\",\n  \"description\": \"Argo CD server version information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Version\": {\n      \"type\": \"string\",\n      \"description\": \"Argo CD version string.\"\n    },\n    \"BuildDate\": {\n      \"type\": \"string\",\n      \"description\": \"Build date.\"\n    },\n    \"GitCommit\": {\n      \"type\": \"string\",\n      \"description\": \"Git commit SHA of this build.\"\n    },\n    \"GoVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Go language version used to build.\"\n    },\n    \"Platform\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system and architecture.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-version-message-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: VersionMessage
---
