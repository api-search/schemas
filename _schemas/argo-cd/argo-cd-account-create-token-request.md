---
description: accountCreateTokenRequest schema from Argo CD API
layout: schema
name: accountCreateTokenRequest
properties_list:
- description: ''
  name: expiresIn
  type: integer
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-account-create-token-request-schema.json
slug: argo-cd-account-create-token-request
source_filename: argo-cd-account-create-token-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-account-create-token-request-schema.json\",\n  \"title\": \"accountCreateTokenRequest\",\n  \"description\": \"accountCreateTokenRequest schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"expiresIn\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"title\": \"expiresIn represents a duration in seconds\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-account-create-token-request-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: accountCreateTokenRequest
---
