---
description: protobufAny schema from Argo CD API
layout: schema
name: protobufAny
properties_list:
- description: ''
  name: type_url
  type: string
- description: ''
  name: value
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-protobuf-any-schema.json
slug: argo-cd-protobuf-any
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-protobuf-any-schema.json\",\n  \"title\": \"protobufAny\",\n  \"description\": \"protobufAny schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type_url\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"format\": \"byte\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-protobuf-any-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: protobufAny
---
