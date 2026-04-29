---
description: oidcClaim schema from Argo CD API
layout: schema
name: oidcClaim
properties_list:
- description: ''
  name: essential
  type: boolean
- description: ''
  name: value
  type: string
- description: ''
  name: values
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-oidc-claim-schema.json
slug: argo-cd-oidc-claim
source_filename: argo-cd-oidc-claim-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-oidc-claim-schema.json\",\n  \"title\": \"oidcClaim\",\n  \"description\": \"oidcClaim schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"essential\": {\n      \"type\": \"boolean\"\n    },\n    \"value\": {\n      \"type\": \"string\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-oidc-claim-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: oidcClaim
---
