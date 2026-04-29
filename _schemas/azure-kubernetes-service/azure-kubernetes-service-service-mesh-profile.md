---
description: Service mesh profile for a managed cluster.
layout: schema
name: ServiceMeshProfile
properties_list:
- description: Mode of the service mesh.
  name: mode
  type: string
- description: Istio service mesh configuration.
  name: istio
  type: object
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-service-mesh-profile-schema.json
slug: azure-kubernetes-service-service-mesh-profile
source_filename: azure-kubernetes-service-service-mesh-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceMeshProfile\",\n  \"type\": \"object\",\n  \"description\": \"Service mesh profile for a managed cluster.\",\n  \"properties\": {\n    \"mode\": {\n      \"type\": \"string\",\n      \"description\": \"Mode of the service mesh.\"\n    },\n    \"istio\": {\n      \"type\": \"object\",\n      \"description\": \"Istio service mesh configuration.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-service-mesh-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ServiceMeshProfile
---
