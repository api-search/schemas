---
description: Workload Auto-scaler profile for the managed cluster.
layout: schema
name: ManagedClusterWorkloadAutoScalerProfile
properties_list:
- description: KEDA (Kubernetes Event-driven Autoscaling) settings.
  name: keda
  type: object
- description: VPA (Vertical Pod Autoscaler) settings.
  name: verticalPodAutoscaler
  type: object
provider_name: Azure Kubernetes Service
provider_slug: microsoft-azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-workload-auto-scaler-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-workload-auto-scaler-profile
source_filename: azure-kubernetes-service-managed-cluster-workload-auto-scaler-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterWorkloadAutoScalerProfile\",\n  \"type\": \"object\",\n  \"description\": \"Workload Auto-scaler profile for the managed cluster.\",\n  \"properties\": {\n    \"keda\": {\n      \"type\": \"object\",\n      \"description\": \"KEDA (Kubernetes Event-driven Autoscaling) settings.\"\n    },\n    \"verticalPodAutoscaler\": {\n      \"type\": \"object\",\n      \"description\": \"VPA (Vertical Pod Autoscaler) settings.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-workload-auto-scaler-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterWorkloadAutoScalerProfile
---
