---
description: v1alpha1ProjectRole schema from Argo CD API
layout: schema
name: v1alpha1ProjectRole
properties_list:
- description: ''
  name: description
  type: string
- description: ''
  name: groups
  type: array
- description: ''
  name: jwtTokens
  type: array
- description: ''
  name: name
  type: string
- description: ''
  name: policies
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-project-role-schema.json
slug: argo-cd-v1alpha1-project-role
source_filename: argo-cd-v1alpha1-project-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-project-role-schema.json\",\n  \"title\": \"v1alpha1ProjectRole\",\n  \"description\": \"v1alpha1ProjectRole schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"title\": \"Description is a description of the role\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"title\": \"Groups are a list of OIDC group claims bound to this role\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"jwtTokens\": {\n      \"type\": \"array\",\n      \"title\": \"JWTTokens are a list of generated JWT tokens bound to this role\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1JWTToken\"\n      }\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name is a\
  \ name for this role\"\n    },\n    \"policies\": {\n      \"type\": \"array\",\n      \"title\": \"Policies Stores a list of casbin formatted strings that define access policies for the role in the project\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-project-role-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ProjectRole
---
