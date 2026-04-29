---
description: Storage profile for the container service cluster.
layout: schema
name: ManagedClusterStorageProfile
properties_list:
- description: ''
  name: diskCSIDriver
  type: object
- description: ''
  name: fileCSIDriver
  type: object
- description: ''
  name: snapshotController
  type: object
- description: ''
  name: blobCSIDriver
  type: object
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-storage-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-storage-profile
source_filename: azure-kubernetes-service-managed-cluster-storage-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterStorageProfile\",\n  \"type\": \"object\",\n  \"description\": \"Storage profile for the container service cluster.\",\n  \"properties\": {\n    \"diskCSIDriver\": {\n      \"type\": \"object\"\n    },\n    \"fileCSIDriver\": {\n      \"type\": \"object\"\n    },\n    \"snapshotController\": {\n      \"type\": \"object\"\n    },\n    \"blobCSIDriver\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-storage-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterStorageProfile
---
