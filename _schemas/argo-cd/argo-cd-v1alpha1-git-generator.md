---
description: v1alpha1GitGenerator schema from Argo CD API
layout: schema
name: v1alpha1GitGenerator
properties_list:
- description: ''
  name: directories
  type: array
- description: ''
  name: files
  type: array
- description: ''
  name: pathParamPrefix
  type: string
- description: ''
  name: repoURL
  type: string
- description: ''
  name: requeueAfterSeconds
  type: integer
- description: ''
  name: revision
  type: string
- description: ''
  name: template
  type: object
- description: ''
  name: values
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-git-generator-schema.json
slug: argo-cd-v1alpha1-git-generator
source_filename: argo-cd-v1alpha1-git-generator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-git-generator-schema.json\",\n  \"title\": \"v1alpha1GitGenerator\",\n  \"description\": \"v1alpha1GitGenerator schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"directories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1GitDirectoryGeneratorItem\"\n      }\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1GitFileGeneratorItem\"\n      }\n    },\n    \"pathParamPrefix\": {\n      \"type\": \"string\"\n    },\n    \"repoURL\": {\n      \"type\": \"string\"\n    },\n    \"requeueAfterSeconds\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"revision\": {\n      \"type\": \"string\"\n    },\n    \"template\": {\n      \"$ref\"\
  : \"#/definitions/v1alpha1ApplicationSetTemplate\"\n    },\n    \"values\": {\n      \"type\": \"object\",\n      \"title\": \"Values contains key/value pairs which are passed directly as parameters to the template\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-git-generator-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1GitGenerator
---
