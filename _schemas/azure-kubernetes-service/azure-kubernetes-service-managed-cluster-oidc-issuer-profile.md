---
description: The OIDC issuer profile of the Managed Cluster.
layout: schema
name: ManagedClusterOIDCIssuerProfile
properties_list:
- description: The OIDC issuer url of the Managed Cluster.
  name: issuerURL
  type: string
- description: Whether the OIDC issuer is enabled.
  name: enabled
  type: boolean
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-managed-cluster-oidc-issuer-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-oidc-issuer-profile
source_filename: azure-kubernetes-service-managed-cluster-oidc-issuer-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterOIDCIssuerProfile\",\n  \"type\": \"object\",\n  \"description\": \"The OIDC issuer profile of the Managed Cluster.\",\n  \"properties\": {\n    \"issuerURL\": {\n      \"type\": \"string\",\n      \"description\": \"The OIDC issuer url of the Managed Cluster.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the OIDC issuer is enabled.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-oidc-issuer-profile-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: ManagedClusterOIDCIssuerProfile
---
