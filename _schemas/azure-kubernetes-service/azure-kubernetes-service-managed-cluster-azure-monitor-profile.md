---
description: Azure Monitor addon profiles for monitoring the managed cluster.
layout: schema
name: ManagedClusterAzureMonitorProfile
properties_list:
- description: Metrics profile for the Azure Monitor managed service for Prometheus addon.
  name: metrics
  type: object
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-azure-monitor-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-azure-monitor-profile
source_filename: azure-kubernetes-service-managed-cluster-azure-monitor-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterAzureMonitorProfile\",\n  \"type\": \"object\",\n  \"description\": \"Azure Monitor addon profiles for monitoring the managed cluster.\",\n  \"properties\": {\n    \"metrics\": {\n      \"type\": \"object\",\n      \"description\": \"Metrics profile for the Azure Monitor managed service for Prometheus addon.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-azure-monitor-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterAzureMonitorProfile
---
