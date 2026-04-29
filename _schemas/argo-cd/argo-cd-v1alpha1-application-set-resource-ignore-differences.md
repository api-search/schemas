---
description: ApplicationSetResourceIgnoreDifferences configures how the ApplicationSet controller will ignore differences in live applications when applying changes from generated applications.
layout: schema
name: v1alpha1ApplicationSetResourceIgnoreDifferences
properties_list:
- description: JQPathExpressions is a list of JQ path expressions to fields to ignore differences for.
  name: jqPathExpressions
  type: array
- description: JSONPointers is a list of JSON pointers to fields to ignore differences for.
  name: jsonPointers
  type: array
- description: Name is the name of the application to ignore differences for. If not specified, the rule applies to all applications.
  name: name
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-resource-ignore-differences-schema.json
slug: argo-cd-v1alpha1-application-set-resource-ignore-differences
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-resource-ignore-differences-schema.json\",\n  \"title\": \"v1alpha1ApplicationSetResourceIgnoreDifferences\",\n  \"description\": \"ApplicationSetResourceIgnoreDifferences configures how the ApplicationSet controller will ignore differences in live\\napplications when applying changes from generated applications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jqPathExpressions\": {\n      \"description\": \"JQPathExpressions is a list of JQ path expressions to fields to ignore differences for.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"jsonPointers\": {\n      \"description\": \"JSONPointers is a list of JSON pointers to fields to ignore differences for.\",\n      \"type\": \"array\",\n      \"items\": {\n \
  \       \"type\": \"string\"\n      }\n    },\n    \"name\": {\n      \"description\": \"Name is the name of the application to ignore differences for. If not specified, the rule applies to all applications.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-resource-ignore-differences-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetResourceIgnoreDifferences
---
