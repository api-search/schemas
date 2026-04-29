---
description: DuckType defines a generator to match against clusters registered with ArgoCD.
layout: schema
name: v1alpha1DuckTypeGenerator
properties_list:
- description: ''
  name: configMapRef
  type: string
- description: ''
  name: labelSelector
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: requeueAfterSeconds
  type: integer
- description: ''
  name: template
  type: object
- description: ''
  name: values
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-duck-type-generator-schema.json
slug: argo-cd-v1alpha1-duck-type-generator
source_filename: argo-cd-v1alpha1-duck-type-generator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-duck-type-generator-schema.json\",\n  \"title\": \"v1alpha1DuckTypeGenerator\",\n  \"description\": \"DuckType defines a generator to match against clusters registered with ArgoCD.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configMapRef\": {\n      \"type\": \"string\",\n      \"title\": \"ConfigMapRef is a ConfigMap with the duck type definitions needed to retrieve the data\\n             this includes apiVersion(group/version), kind, matchKey and validation settings\\nName is the resource name of the kind, group and version, defined in the ConfigMapRef\\nRequeueAfterSeconds is how long before the duckType will be rechecked for a change\"\n    },\n    \"labelSelector\": {\n      \"$ref\": \"#/definitions/v1LabelSelector\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n   \
  \ },\n    \"requeueAfterSeconds\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"template\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSetTemplate\"\n    },\n    \"values\": {\n      \"type\": \"object\",\n      \"title\": \"Values contains key/value pairs which are passed directly as parameters to the template\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-duck-type-generator-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1DuckTypeGenerator
---
