---
description: v1alpha1ApplicationSetTree schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSetTree
properties_list:
- description: ''
  name: nodes
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-tree-schema.json
slug: argo-cd-v1alpha1-application-set-tree
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-tree-schema.json\",\n  \"title\": \"v1alpha1ApplicationSetTree\",\n  \"description\": \"v1alpha1ApplicationSetTree schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nodes\": {\n      \"type\": \"array\",\n      \"title\": \"Nodes contains list of nodes which are directly managed by the applicationset\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ResourceNode\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-tree-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetTree
---
