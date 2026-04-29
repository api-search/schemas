---
description: v1alpha1ApplicationSourceJsonnet schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSourceJsonnet
properties_list:
- description: ''
  name: extVars
  type: array
- description: ''
  name: libs
  type: array
- description: ''
  name: tlas
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-source-jsonnet-schema.json
slug: argo-cd-v1alpha1-application-source-jsonnet
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-source-jsonnet-schema.json\",\n  \"title\": \"v1alpha1ApplicationSourceJsonnet\",\n  \"description\": \"v1alpha1ApplicationSourceJsonnet schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"extVars\": {\n      \"type\": \"array\",\n      \"title\": \"ExtVars is a list of Jsonnet External Variables\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1JsonnetVar\"\n      }\n    },\n    \"libs\": {\n      \"type\": \"array\",\n      \"title\": \"Additional library search dirs\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tlas\": {\n      \"type\": \"array\",\n      \"title\": \"TLAS is a list of Jsonnet Top-level Arguments\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1JsonnetVar\"\n      }\n   \
  \ }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-source-jsonnet-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSourceJsonnet
---
