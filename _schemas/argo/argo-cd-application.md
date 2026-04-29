---
description: An Argo CD Application represents a deployed set of Kubernetes resources managed through GitOps.
layout: schema
name: Application
properties_list:
- description: API version, always argoproj.io/v1alpha1.
  name: apiVersion
  type: string
- description: Resource kind, always Application.
  name: kind
  type: string
- description: Kubernetes object metadata.
  name: metadata
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: status
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-application-schema.json
slug: argo-cd-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-application-schema.json\",\n  \"title\": \"Application\",\n  \"description\": \"An Argo CD Application represents a deployed set of Kubernetes resources managed through GitOps.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"description\": \"API version, always argoproj.io/v1alpha1.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Resource kind, always Application.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Kubernetes object metadata.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Application name.\"\n        },\n        \"namespace\": {\n          \"type\": \"string\",\n          \"description\": \"Application\
  \ namespace.\"\n        }\n      }\n    },\n    \"spec\": {\n      \"$ref\": \"#/components/schemas/ApplicationSpec\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/ApplicationStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-application-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Application
---
