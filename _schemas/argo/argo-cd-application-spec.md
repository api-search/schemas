---
description: Desired state specification for an Argo CD application.
layout: schema
name: ApplicationSpec
properties_list:
- description: ''
  name: source
  type: object
- description: ''
  name: destination
  type: object
- description: Argo CD project this application belongs to.
  name: project
  type: string
- description: ''
  name: syncPolicy
  type: object
- description: Resource fields to ignore when computing sync status.
  name: ignoreDifferences
  type: array
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-application-spec-schema.json
slug: argo-cd-application-spec
source_filename: argo-cd-application-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-application-spec-schema.json\",\n  \"title\": \"ApplicationSpec\",\n  \"description\": \"Desired state specification for an Argo CD application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"$ref\": \"#/components/schemas/ApplicationSource\"\n    },\n    \"destination\": {\n      \"$ref\": \"#/components/schemas/ApplicationDestination\"\n    },\n    \"project\": {\n      \"type\": \"string\",\n      \"description\": \"Argo CD project this application belongs to.\"\n    },\n    \"syncPolicy\": {\n      \"$ref\": \"#/components/schemas/SyncPolicy\"\n    },\n    \"ignoreDifferences\": {\n      \"type\": \"array\",\n      \"description\": \"Resource fields to ignore when computing sync status.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n   \
  \       \"group\": {\n            \"type\": \"string\",\n            \"description\": \"Kubernetes API group.\"\n          },\n          \"kind\": {\n            \"type\": \"string\",\n            \"description\": \"Kubernetes resource kind.\"\n          },\n          \"jsonPointers\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"JSON Pointer paths to ignore.\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"destination\",\n    \"project\",\n    \"source\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-application-spec-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: ApplicationSpec
---
