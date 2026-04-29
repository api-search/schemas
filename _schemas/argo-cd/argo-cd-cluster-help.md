---
description: clusterHelp schema from Argo CD API
layout: schema
name: clusterHelp
properties_list:
- description: ''
  name: binaryUrls
  type: object
- description: ''
  name: chatText
  type: string
- description: ''
  name: chatUrl
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-cluster-help-schema.json
slug: argo-cd-cluster-help
source_filename: argo-cd-cluster-help-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-cluster-help-schema.json\",\n  \"title\": \"clusterHelp\",\n  \"description\": \"clusterHelp schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"binaryUrls\": {\n      \"type\": \"object\",\n      \"title\": \"the URLs for downloading argocd binaries\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"chatText\": {\n      \"type\": \"string\",\n      \"title\": \"the text for getting chat help, defaults to \\\"Chat now!\\\"\"\n    },\n    \"chatUrl\": {\n      \"type\": \"string\",\n      \"title\": \"the URL for getting chat help, this will typically be your Slack channel for support\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-cluster-help-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: clusterHelp
---
