---
description: applicationResourceActionRunRequestV2 schema from Argo CD API
layout: schema
name: applicationResourceActionRunRequestV2
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: appNamespace
  type: string
- description: ''
  name: group
  type: string
- description: ''
  name: kind
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: project
  type: string
- description: ''
  name: resourceActionParameters
  type: array
- description: ''
  name: resourceName
  type: string
- description: ''
  name: version
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-application-resource-action-run-request-v2-schema.json
slug: argo-cd-application-resource-action-run-request-v2
source_filename: argo-cd-application-resource-action-run-request-v2-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-resource-action-run-request-v2-schema.json\",\n  \"title\": \"applicationResourceActionRunRequestV2\",\n  \"description\": \"applicationResourceActionRunRequestV2 schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\"\n    },\n    \"appNamespace\": {\n      \"type\": \"string\"\n    },\n    \"group\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"project\": {\n      \"type\": \"string\"\n    },\n    \"resourceActionParameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/applicationResourceActionParameters\"\n      }\n    },\n\
  \    \"resourceName\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-resource-action-run-request-v2-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: applicationResourceActionRunRequestV2
---
