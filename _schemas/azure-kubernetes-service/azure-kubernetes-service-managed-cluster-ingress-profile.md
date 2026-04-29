---
description: Ingress profile for the managed cluster.
layout: schema
name: ManagedClusterIngressProfile
properties_list:
- description: Web App Routing settings.
  name: webAppRouting
  type: object
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-ingress-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-ingress-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterIngressProfile\",\n  \"type\": \"object\",\n  \"description\": \"Ingress profile for the managed cluster.\",\n  \"properties\": {\n    \"webAppRouting\": {\n      \"type\": \"object\",\n      \"description\": \"Web App Routing settings.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-ingress-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterIngressProfile
---
