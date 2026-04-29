---
description: 'JSON represents any valid JSON value. These types are supported: bool, int64, float64, string, []interface{}, map[string]interface{} and nil.'
layout: schema
name: v1JSON
properties_list:
- description: ''
  name: raw
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-json-schema.json
slug: argo-cd-v1-json
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-json-schema.json\",\n  \"title\": \"v1JSON\",\n  \"description\": \"JSON represents any valid JSON value.\\nThese types are supported: bool, int64, float64, string, []interface{}, map[string]interface{} and nil.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"raw\": {\n      \"type\": \"string\",\n      \"format\": \"byte\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-json-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1JSON
---
