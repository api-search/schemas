---
description: v1alpha1Cluster schema from Argo CD API
layout: schema
name: v1alpha1Cluster
properties_list:
- description: ''
  name: annotations
  type: object
- description: Indicates if cluster level resources should be managed. This setting is used only if cluster is connected in a namespaced mode.
  name: clusterResources
  type: boolean
- description: ''
  name: config
  type: object
- description: ''
  name: connectionState
  type: object
- description: ''
  name: info
  type: object
- description: ''
  name: labels
  type: object
- description: ''
  name: name
  type: string
- description: Holds list of namespaces which are accessible in that cluster. Cluster level resources will be ignored if namespace list is not empty.
  name: namespaces
  type: array
- description: ''
  name: project
  type: string
- description: ''
  name: refreshRequestedAt
  type: object
- description: ''
  name: server
  type: string
- description: ''
  name: serverVersion
  type: string
- description: Shard contains optional shard number. Calculated on the fly by the application controller if not specified.
  name: shard
  type: integer
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-cluster-schema.json
slug: argo-cd-v1alpha1-cluster
source_filename: argo-cd-v1alpha1-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-cluster-schema.json\",\n  \"title\": \"v1alpha1Cluster\",\n  \"description\": \"v1alpha1Cluster schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"annotations\": {\n      \"type\": \"object\",\n      \"title\": \"Annotations for cluster secret metadata\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"clusterResources\": {\n      \"description\": \"Indicates if cluster level resources should be managed. This setting is used only if cluster is connected in a namespaced mode.\",\n      \"type\": \"boolean\"\n    },\n    \"config\": {\n      \"$ref\": \"#/definitions/v1alpha1ClusterConfig\"\n    },\n    \"connectionState\": {\n      \"$ref\": \"#/definitions/v1alpha1ConnectionState\"\n    },\n    \"info\": {\n      \"$ref\": \"\
  #/definitions/v1alpha1ClusterInfo\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"title\": \"Labels for cluster secret metadata\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name of the cluster. If omitted, will use the server address\"\n    },\n    \"namespaces\": {\n      \"description\": \"Holds list of namespaces which are accessible in that cluster. Cluster level resources will be ignored if namespace list is not empty.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"project\": {\n      \"type\": \"string\",\n      \"title\": \"Reference between project and cluster that allow you automatically to be added as item inside Destinations project entity\"\n    },\n    \"refreshRequestedAt\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"server\": {\n      \"type\": \"string\",\n      \"title\": \"\
  Server is the API server URL of the Kubernetes cluster\"\n    },\n    \"serverVersion\": {\n      \"type\": \"string\",\n      \"title\": \"Deprecated: use Info.ServerVersion field instead.\\nThe server version\"\n    },\n    \"shard\": {\n      \"description\": \"Shard contains optional shard number. Calculated on the fly by the application controller if not specified.\",\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-cluster-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1Cluster
---
