---
description: A node selector requirement is a selector that contains values, a key, and an operator that relates the key and values.
layout: schema
name: io.k8s.api.core.v1.NodeSelectorRequirement
properties_list:
- description: The label key that the selector applies to.
  name: key
  type: string
- description: Represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists, DoesNotExist. Gt, and Lt.
  name: operator
  type: string
- description: An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, t
  name: values
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-node-selector-requirement-schema.json
slug: argo-workflows-io-k8s-api-core-v1-node-selector-requirement
source_filename: argo-workflows-io-k8s-api-core-v1-node-selector-requirement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-node-selector-requirement-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.NodeSelectorRequirement\",\n  \"description\": \"A node selector requirement is a selector that contains values, a key, and an operator that relates the key and values.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"description\": \"The label key that the selector applies to.\",\n      \"type\": \"string\"\n    },\n    \"operator\": {\n      \"description\": \"Represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists, DoesNotExist. Gt, and Lt.\",\n      \"type\": \"string\"\n    },\n    \"values\": {\n      \"description\": \"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is\
  \ Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    }\n  },\n  \"required\": [\n    \"key\",\n    \"operator\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-node-selector-requirement-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.NodeSelectorRequirement
---
