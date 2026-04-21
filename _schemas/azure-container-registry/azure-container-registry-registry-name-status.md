---
description: The result of a request to check the availability of a container registry name.
layout: schema
name: RegistryNameStatus
properties_list:
- description: If any, the error message that provides more detail for the reason that the name is not available.
  name: message
  type: string
- description: The value that indicates whether the name is available.
  name: nameAvailable
  type: boolean
- description: If any, the reason that the name is not available.
  name: reason
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-registry-name-status-schema.json
slug: azure-container-registry-registry-name-status
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: RegistryNameStatus
---
