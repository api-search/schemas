---
description: v1alpha1ClusterInfo schema from Argo CD API
layout: schema
name: v1alpha1ClusterInfo
properties_list:
- description: ''
  name: apiVersions
  type: array
- description: ''
  name: applicationsCount
  type: integer
- description: ''
  name: cacheInfo
  type: object
- description: ''
  name: connectionState
  type: object
- description: ''
  name: serverVersion
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-cluster-info-schema.json
slug: argo-cd-v1alpha1-cluster-info
source_filename: argo-cd-v1alpha1-cluster-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-cluster-info-schema.json\",\n  \"title\": \"v1alpha1ClusterInfo\",\n  \"description\": \"v1alpha1ClusterInfo schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersions\": {\n      \"type\": \"array\",\n      \"title\": \"APIVersions contains list of API versions supported by the cluster\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"applicationsCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"title\": \"ApplicationsCount is the number of applications managed by Argo CD on the cluster\"\n    },\n    \"cacheInfo\": {\n      \"$ref\": \"#/definitions/v1alpha1ClusterCacheInfo\"\n    },\n    \"connectionState\": {\n      \"$ref\": \"#/definitions/v1alpha1ConnectionState\"\n    },\n    \"serverVersion\": {\n\
  \      \"type\": \"string\",\n      \"title\": \"ServerVersion contains information about the Kubernetes version of the cluster\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-cluster-info-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ClusterInfo
---
