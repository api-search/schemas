---
description: A label selector is a label query over a set of resources. The result of matchLabels and matchExpressions are ANDed. An empty label selector matches all objects. A null label selector matches no objects.
layout: schema
name: io.k8s.apimachinery.pkg.apis.meta.v1.LabelSelector
properties_list:
- description: matchExpressions is a list of label selector requirements. The requirements are ANDed.
  name: matchExpressions
  type: array
- description: matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is "key", the operator is "In", and the values a
  name: matchLabels
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-label-selector-schema.json
slug: argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-label-selector
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-label-selector-schema.json\",\n  \"title\": \"io.k8s.apimachinery.pkg.apis.meta.v1.LabelSelector\",\n  \"description\": \"A label selector is a label query over a set of resources. The result of matchLabels and matchExpressions are ANDed. An empty label selector matches all objects. A null label selector matches no objects.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"matchExpressions\": {\n      \"description\": \"matchExpressions is a list of label selector requirements. The requirements are ANDed.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.LabelSelectorRequirement\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"matchLabels\": {\n     \
  \ \"description\": \"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \\\"key\\\", the operator is \\\"In\\\", and the values array contains only \\\"value\\\". The requirements are ANDed.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-label-selector-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.apimachinery.pkg.apis.meta.v1.LabelSelector
---
