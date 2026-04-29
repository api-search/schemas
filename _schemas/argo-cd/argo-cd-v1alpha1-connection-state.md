---
description: v1alpha1ConnectionState schema from Argo CD API
layout: schema
name: v1alpha1ConnectionState
properties_list:
- description: ''
  name: attemptedAt
  type: object
- description: ''
  name: message
  type: string
- description: ''
  name: status
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-connection-state-schema.json
slug: argo-cd-v1alpha1-connection-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-connection-state-schema.json\",\n  \"title\": \"v1alpha1ConnectionState\",\n  \"description\": \"v1alpha1ConnectionState schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attemptedAt\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"title\": \"Message contains human readable information about the connection status\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"title\": \"Status contains the current status indicator for the connection\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-connection-state-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ConnectionState
---
