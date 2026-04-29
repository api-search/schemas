---
description: +protobuf=true +protobuf.options.(gogoproto.goproto_stringer)=false +k8s:openapi-gen=true
layout: schema
name: intstrIntOrString
properties_list:
- description: ''
  name: intVal
  type: integer
- description: ''
  name: strVal
  type: string
- description: ''
  name: type
  type: integer
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-intstr-int-or-string-schema.json
slug: argo-cd-intstr-int-or-string
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-intstr-int-or-string-schema.json\",\n  \"title\": \"intstrIntOrString\",\n  \"description\": \"+protobuf=true\\n+protobuf.options.(gogoproto.goproto_stringer)=false\\n+k8s:openapi-gen=true\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"intVal\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"strVal\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-intstr-int-or-string-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: intstrIntOrString
---
