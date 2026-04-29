---
description: An Argo Workflow resource
layout: schema
name: Workflow
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
- description: ''
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
schema_file: json-schema/argo-workflows-workflow-schema.json
slug: argo-workflows-workflow
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-schema.json\",\n  \"title\": \"Workflow\",\n  \"description\": \"An Argo Workflow resource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"default\": \"argoproj.io/v1alpha1\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"default\": \"Workflow\"\n    },\n    \"metadata\": {\n      \"$ref\": \"#/components/schemas/ObjectMeta\"\n    },\n    \"spec\": {\n      \"$ref\": \"#/components/schemas/WorkflowSpec\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/WorkflowStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Workflow
---
