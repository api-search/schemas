---
description: repositoryHelmAppSpec schema from Argo CD API
layout: schema
name: repositoryHelmAppSpec
properties_list:
- description: ''
  name: fileParameters
  type: array
- description: ''
  name: name
  type: string
- description: ''
  name: parameters
  type: array
- description: ''
  name: valueFiles
  type: array
- description: ''
  name: values
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-repository-helm-app-spec-schema.json
slug: argo-cd-repository-helm-app-spec
source_filename: argo-cd-repository-helm-app-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-helm-app-spec-schema.json\",\n  \"title\": \"repositoryHelmAppSpec\",\n  \"description\": \"repositoryHelmAppSpec schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileParameters\": {\n      \"type\": \"array\",\n      \"title\": \"helm file parameters\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1HelmFileParameter\"\n      }\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"title\": \"the output of `helm inspect values`\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1HelmParameter\"\n      }\n    },\n    \"valueFiles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"values\": {\n      \"type\": \"\
  string\",\n      \"title\": \"the contents of values.yaml\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-helm-app-spec-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: repositoryHelmAppSpec
---
