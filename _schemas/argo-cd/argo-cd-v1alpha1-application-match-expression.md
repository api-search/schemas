---
description: v1alpha1ApplicationMatchExpression schema from Argo CD API
layout: schema
name: v1alpha1ApplicationMatchExpression
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: operator
  type: string
- description: ''
  name: values
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-match-expression-schema.json
slug: argo-cd-v1alpha1-application-match-expression
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-match-expression-schema.json\",\n  \"title\": \"v1alpha1ApplicationMatchExpression\",\n  \"description\": \"v1alpha1ApplicationMatchExpression schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"operator\": {\n      \"type\": \"string\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-match-expression-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationMatchExpression
---
