---
description: A Kubernetes add-on profile for a managed cluster.
layout: schema
name: ManagedClusterAddonProfile
properties_list:
- description: Whether the add-on is enabled.
  name: enabled
  type: boolean
- description: Key-value pairs for configuring an add-on.
  name: config
  type: object
- description: ''
  name: identity
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-kubernetes-service-managed-cluster-addon-profile-schema.json
slug: azure-kubernetes-service-managed-cluster-addon-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedClusterAddonProfile\",\n  \"type\": \"object\",\n  \"description\": \"A Kubernetes add-on profile for a managed cluster.\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the add-on is enabled.\"\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs for configuring an add-on.\"\n    },\n    \"identity\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-addon-profile-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ManagedClusterAddonProfile
---
