---
description: Access profile for managed cluster API server.
layout: schema
name: ManagedClusterAPIServerAccessProfile
properties_list:
- description: IP ranges authorized to access the Kubernetes API server.
  name: authorizedIPRanges
  type: array
- description: Whether to create the cluster as a private cluster or not.
  name: enablePrivateCluster
  type: boolean
- description: The private DNS zone mode for the cluster.
  name: privateDNSZone
  type: string
- description: Whether to create a public FQDN for private cluster or not.
  name: enablePrivateClusterPublicFQDN
  type: boolean
- description: Whether to disable run command for the cluster.
  name: disableRunCommand
  type: boolean
- description: Whether to enable API server VNET integration for the cluster.
  name: enableVnetIntegration
  type: boolean
- description: The subnet to be used when API server VNET integration is enabled.
  name: subnetId
  type: string
provider_name: Azure Kubernetes Service
provider_slug: microsoft-azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-api-server-access-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-api-server-access-profile
source_filename: azure-kubernetes-service-managed-cluster-api-server-access-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterAPIServerAccessProfile\",\n  \"type\": \"object\",\n  \"description\": \"Access profile for managed cluster API server.\",\n  \"properties\": {\n    \"authorizedIPRanges\": {\n      \"type\": \"array\",\n      \"description\": \"IP ranges authorized to access the Kubernetes API server.\"\n    },\n    \"enablePrivateCluster\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to create the cluster as a private cluster or not.\"\n    },\n    \"privateDNSZone\": {\n      \"type\": \"string\",\n      \"description\": \"The private DNS zone mode for the cluster.\"\n    },\n    \"enablePrivateClusterPublicFQDN\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to create a public FQDN for private cluster or not.\"\n    },\n    \"disableRunCommand\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to disable run command for the cluster.\"\
  \n    },\n    \"enableVnetIntegration\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable API server VNET integration for the cluster.\"\n    },\n    \"subnetId\": {\n      \"type\": \"string\",\n      \"description\": \"The subnet to be used when API server VNET integration is enabled.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-api-server-access-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterAPIServerAccessProfile
---
