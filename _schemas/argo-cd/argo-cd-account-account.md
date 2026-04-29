---
description: accountAccount schema from Argo CD API
layout: schema
name: accountAccount
properties_list:
- description: ''
  name: capabilities
  type: array
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: tokens
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-account-account-schema.json
slug: argo-cd-account-account
source_filename: argo-cd-account-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-account-account-schema.json\",\n  \"title\": \"accountAccount\",\n  \"description\": \"accountAccount schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"capabilities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"tokens\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/accountToken\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-account-account-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: accountAccount
---
