---
description: v1LabelSelector schema from Argo CD API
layout: schema
name: v1LabelSelector
properties_list:
- description: ''
  name: matchExpressions
  type: array
- description: ''
  name: matchLabels
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-label-selector-schema.json
slug: argo-cd-v1-label-selector
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-label-selector-schema.json\",\n  \"title\": \"v1LabelSelector\",\n  \"description\": \"v1LabelSelector schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"matchExpressions\": {\n      \"type\": \"array\",\n      \"title\": \"matchExpressions is a list of label selector requirements. The requirements are ANDed.\\n+optional\\n+listType=atomic\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1LabelSelectorRequirement\"\n      }\n    },\n    \"matchLabels\": {\n      \"type\": \"object\",\n      \"title\": \"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\\nmap is equivalent to an element of matchExpressions, whose key field is \\\"key\\\", the\\noperator is \\\"In\\\", and the values array contains only \\\"value\\\". The requirements\
  \ are ANDed.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-label-selector-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1LabelSelector
---
