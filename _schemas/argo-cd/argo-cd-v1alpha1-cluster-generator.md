---
description: ClusterGenerator defines a generator to match against clusters registered with ArgoCD.
layout: schema
name: v1alpha1ClusterGenerator
properties_list:
- description: ''
  name: flatList
  type: boolean
- description: ''
  name: selector
  type: object
- description: ''
  name: template
  type: object
- description: ''
  name: values
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-cluster-generator-schema.json
slug: argo-cd-v1alpha1-cluster-generator
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-cluster-generator-schema.json\",\n  \"title\": \"v1alpha1ClusterGenerator\",\n  \"description\": \"ClusterGenerator defines a generator to match against clusters registered with ArgoCD.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flatList\": {\n      \"type\": \"boolean\",\n      \"title\": \"returns the clusters a single 'clusters' value in the template\"\n    },\n    \"selector\": {\n      \"$ref\": \"#/definitions/v1LabelSelector\"\n    },\n    \"template\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSetTemplate\"\n    },\n    \"values\": {\n      \"type\": \"object\",\n      \"title\": \"Values contains key/value pairs which are passed directly as parameters to the template\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-cluster-generator-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ClusterGenerator
---
