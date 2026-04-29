---
description: Security profile for the container service cluster.
layout: schema
name: ManagedClusterSecurityProfile
properties_list:
- description: Microsoft Defender settings for the security profile.
  name: defender
  type: object
- description: Workload identity settings for the security profile.
  name: workloadIdentity
  type: object
- description: Image Cleaner settings for the security profile.
  name: imageCleaner
  type: object
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-security-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-security-profile
source_filename: azure-kubernetes-service-managed-cluster-security-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterSecurityProfile\",\n  \"type\": \"object\",\n  \"description\": \"Security profile for the container service cluster.\",\n  \"properties\": {\n    \"defender\": {\n      \"type\": \"object\",\n      \"description\": \"Microsoft Defender settings for the security profile.\"\n    },\n    \"workloadIdentity\": {\n      \"type\": \"object\",\n      \"description\": \"Workload identity settings for the security profile.\"\n    },\n    \"imageCleaner\": {\n      \"type\": \"object\",\n      \"description\": \"Image Cleaner settings for the security profile.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-security-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterSecurityProfile
---
