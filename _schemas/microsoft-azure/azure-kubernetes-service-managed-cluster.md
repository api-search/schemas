---
description: Managed cluster resource.
layout: schema
name: ManagedCluster
properties_list:
- description: Resource ID.
  name: id
  type: string
- description: Resource name.
  name: name
  type: string
- description: Resource type.
  name: type
  type: string
- description: The geo-location where the resource lives.
  name: location
  type: string
- description: Resource tags.
  name: tags
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-kubernetes-service-managed-cluster-schema.json
slug: azure-kubernetes-service-managed-cluster
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedCluster\",\n  \"type\": \"object\",\n  \"description\": \"Managed cluster resource.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Resource ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The geo-location where the resource lives.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Resource tags.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-kubernetes-service-managed-cluster-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ManagedCluster
---
