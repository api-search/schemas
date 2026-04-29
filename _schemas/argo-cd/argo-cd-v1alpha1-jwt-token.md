---
description: v1alpha1JWTToken schema from Argo CD API
layout: schema
name: v1alpha1JWTToken
properties_list:
- description: ''
  name: exp
  type: integer
- description: ''
  name: iat
  type: integer
- description: ''
  name: id
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-jwt-token-schema.json
slug: argo-cd-v1alpha1-jwt-token
source_filename: argo-cd-v1alpha1-jwt-token-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-jwt-token-schema.json\",\n  \"title\": \"v1alpha1JWTToken\",\n  \"description\": \"v1alpha1JWTToken schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exp\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"iat\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-jwt-token-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1JWTToken
---
