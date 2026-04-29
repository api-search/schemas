---
description: sessionGetUserInfoResponse schema from Argo CD API
layout: schema
name: sessionGetUserInfoResponse
properties_list:
- description: ''
  name: groups
  type: array
- description: ''
  name: iss
  type: string
- description: ''
  name: loggedIn
  type: boolean
- description: ''
  name: username
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-session-get-user-info-response-schema.json
slug: argo-cd-session-get-user-info-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-session-get-user-info-response-schema.json\",\n  \"title\": \"sessionGetUserInfoResponse\",\n  \"description\": \"sessionGetUserInfoResponse schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"iss\": {\n      \"type\": \"string\"\n    },\n    \"loggedIn\": {\n      \"type\": \"boolean\"\n    },\n    \"username\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-session-get-user-info-response-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: sessionGetUserInfoResponse
---
