---
description: v1alpha1OverrideIgnoreDiff schema from Argo CD API
layout: schema
name: v1alpha1OverrideIgnoreDiff
properties_list:
- description: ''
  name: jSONPointers
  type: array
- description: ''
  name: jqPathExpressions
  type: array
- description: ''
  name: managedFieldsManagers
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-override-ignore-diff-schema.json
slug: argo-cd-v1alpha1-override-ignore-diff
source_filename: argo-cd-v1alpha1-override-ignore-diff-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-override-ignore-diff-schema.json\",\n  \"title\": \"v1alpha1OverrideIgnoreDiff\",\n  \"description\": \"v1alpha1OverrideIgnoreDiff schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jSONPointers\": {\n      \"type\": \"array\",\n      \"title\": \"JSONPointers is a JSON path list following the format defined in RFC4627 (https://datatracker.ietf.org/doc/html/rfc6902#section-3)\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"jqPathExpressions\": {\n      \"type\": \"array\",\n      \"title\": \"JQPathExpressions is a JQ path list that will be evaludated during the diff process\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"managedFieldsManagers\": {\n      \"type\": \"array\",\n      \"title\": \"ManagedFieldsManagers\
  \ is a list of trusted managers. Fields mutated by those managers will take precedence over the\\ndesired state defined in the SCM and won't be displayed in diffs\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-override-ignore-diff-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1OverrideIgnoreDiff
---
