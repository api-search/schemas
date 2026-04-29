---
description: v1alpha1ClusterCacheInfo schema from Argo CD API
layout: schema
name: v1alpha1ClusterCacheInfo
properties_list:
- description: ''
  name: apisCount
  type: integer
- description: ''
  name: lastCacheSyncTime
  type: object
- description: ''
  name: resourcesCount
  type: integer
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-cluster-cache-info-schema.json
slug: argo-cd-v1alpha1-cluster-cache-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-cluster-cache-info-schema.json\",\n  \"title\": \"v1alpha1ClusterCacheInfo\",\n  \"description\": \"v1alpha1ClusterCacheInfo schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apisCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"title\": \"APIsCount holds number of observed Kubernetes API count\"\n    },\n    \"lastCacheSyncTime\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"resourcesCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"title\": \"ResourcesCount holds number of observed Kubernetes resources\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-cluster-cache-info-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ClusterCacheInfo
---
