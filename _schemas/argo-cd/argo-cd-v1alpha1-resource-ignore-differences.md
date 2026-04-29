---
description: ResourceIgnoreDifferences contains resource filter and list of json paths which should be ignored during comparison with live state.
layout: schema
name: v1alpha1ResourceIgnoreDifferences
properties_list:
- description: ''
  name: group
  type: string
- description: ''
  name: jqPathExpressions
  type: array
- description: ''
  name: jsonPointers
  type: array
- description: ''
  name: kind
  type: string
- description: ''
  name: managedFieldsManagers
  type: array
- description: ''
  name: name
  type: string
- description: ''
  name: namespace
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-resource-ignore-differences-schema.json
slug: argo-cd-v1alpha1-resource-ignore-differences
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-resource-ignore-differences-schema.json\",\n  \"title\": \"v1alpha1ResourceIgnoreDifferences\",\n  \"description\": \"ResourceIgnoreDifferences contains resource filter and list of json paths which should be ignored during comparison with live state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"group\": {\n      \"type\": \"string\"\n    },\n    \"jqPathExpressions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"jsonPointers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"managedFieldsManagers\": {\n      \"type\": \"array\",\n      \"title\": \"ManagedFieldsManagers is a list of trusted managers. Fields mutated by\
  \ those managers will take precedence over the\\ndesired state defined in the SCM and won't be displayed in diffs\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-resource-ignore-differences-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ResourceIgnoreDifferences
---
