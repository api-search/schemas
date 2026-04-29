---
description: A label selector requirement is a selector that contains values, a key, and an operator that relates the key and values.
layout: schema
name: v1LabelSelectorRequirement
properties_list:
- description: key is the label key that the selector applies to.
  name: key
  type: string
- description: operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist.
  name: operator
  type: string
- description: ''
  name: values
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-label-selector-requirement-schema.json
slug: argo-cd-v1-label-selector-requirement
source_filename: argo-cd-v1-label-selector-requirement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-label-selector-requirement-schema.json\",\n  \"title\": \"v1LabelSelectorRequirement\",\n  \"description\": \"A label selector requirement is a selector that contains values, a key, and an operator that\\nrelates the key and values.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"description\": \"key is the label key that the selector applies to.\",\n      \"type\": \"string\"\n    },\n    \"operator\": {\n      \"description\": \"operator represents a key's relationship to a set of values.\\nValid operators are In, NotIn, Exists and DoesNotExist.\",\n      \"type\": \"string\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"title\": \"values is an array of string values. If the operator is In or NotIn,\\nthe values array must be non-empty. If the operator is\
  \ Exists or DoesNotExist,\\nthe values array must be empty. This array is replaced during a strategic\\nmerge patch.\\n+optional\\n+listType=atomic\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-label-selector-requirement-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1LabelSelectorRequirement
---
