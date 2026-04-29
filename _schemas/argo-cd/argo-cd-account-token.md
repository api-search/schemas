---
description: accountToken schema from Argo CD API
layout: schema
name: accountToken
properties_list:
- description: ''
  name: expiresAt
  type: integer
- description: ''
  name: id
  type: string
- description: ''
  name: issuedAt
  type: integer
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-account-token-schema.json
slug: argo-cd-account-token
source_filename: argo-cd-account-token-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-account-token-schema.json\",\n  \"title\": \"accountToken\",\n  \"description\": \"accountToken schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"expiresAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"issuedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-account-token-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: accountToken
---
