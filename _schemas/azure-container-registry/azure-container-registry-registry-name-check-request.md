---
description: A request to check whether a container registry name is available.
layout: schema
name: RegistryNameCheckRequest
properties_list:
- description: The name of the container registry.
  name: name
  type: string
- description: The resource type of the container registry. This field must be set to 'Microsoft.ContainerRegistry/registries'.
  name: type
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-registry-name-check-request-schema.json
slug: azure-container-registry-registry-name-check-request
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: RegistryNameCheckRequest
---
