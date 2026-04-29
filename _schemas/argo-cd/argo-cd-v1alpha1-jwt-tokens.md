---
description: v1alpha1JWTTokens schema from Argo CD API
layout: schema
name: v1alpha1JWTTokens
properties_list:
- description: ''
  name: items
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-jwt-tokens-schema.json
slug: argo-cd-v1alpha1-jwt-tokens
source_filename: argo-cd-v1alpha1-jwt-tokens-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-jwt-tokens-schema.json\",\n  \"title\": \"v1alpha1JWTTokens\",\n  \"description\": \"v1alpha1JWTTokens schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1JWTToken\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-jwt-tokens-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1JWTTokens
---
