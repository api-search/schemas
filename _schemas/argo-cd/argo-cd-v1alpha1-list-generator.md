---
description: v1alpha1ListGenerator schema from Argo CD API
layout: schema
name: v1alpha1ListGenerator
properties_list:
- description: ''
  name: elements
  type: array
- description: ''
  name: elementsYaml
  type: string
- description: ''
  name: template
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-list-generator-schema.json
slug: argo-cd-v1alpha1-list-generator
source_filename: argo-cd-v1alpha1-list-generator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-list-generator-schema.json\",\n  \"title\": \"v1alpha1ListGenerator\",\n  \"description\": \"v1alpha1ListGenerator schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"elements\": {\n      \"type\": \"array\",\n      \"title\": \"+kubebuilder:validation:Optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1JSON\"\n      }\n    },\n    \"elementsYaml\": {\n      \"type\": \"string\"\n    },\n    \"template\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSetTemplate\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-list-generator-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ListGenerator
---
