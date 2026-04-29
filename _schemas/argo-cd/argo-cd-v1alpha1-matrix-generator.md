---
description: MatrixGenerator generates the cartesian product of two sets of parameters. The parameters are defined by two nested generators.
layout: schema
name: v1alpha1MatrixGenerator
properties_list:
- description: ''
  name: generators
  type: array
- description: ''
  name: template
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-matrix-generator-schema.json
slug: argo-cd-v1alpha1-matrix-generator
source_filename: argo-cd-v1alpha1-matrix-generator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-matrix-generator-schema.json\",\n  \"title\": \"v1alpha1MatrixGenerator\",\n  \"description\": \"MatrixGenerator generates the cartesian product of two sets of parameters. The parameters are defined by two nested\\ngenerators.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"generators\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationSetNestedGenerator\"\n      }\n    },\n    \"template\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSetTemplate\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-matrix-generator-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1MatrixGenerator
---
