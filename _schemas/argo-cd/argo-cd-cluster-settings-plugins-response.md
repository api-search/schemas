---
description: clusterSettingsPluginsResponse schema from Argo CD API
layout: schema
name: clusterSettingsPluginsResponse
properties_list:
- description: ''
  name: plugins
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-cluster-settings-plugins-response-schema.json
slug: argo-cd-cluster-settings-plugins-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-cluster-settings-plugins-response-schema.json\",\n  \"title\": \"clusterSettingsPluginsResponse\",\n  \"description\": \"clusterSettingsPluginsResponse schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"plugins\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/clusterPlugin\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-cluster-settings-plugins-response-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: clusterSettingsPluginsResponse
---
