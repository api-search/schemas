---
description: ImportSource schema from Azure Container Registry API
layout: schema
name: ImportSource
properties_list:
- description: Credentials used when importing from a registry uri.
  name: credentials
  type: object
- description: The address of the source registry (e.g. 'mcr.microsoft.com').
  name: registryUri
  type: string
- description: The resource identifier of the source Azure Container Registry.
  name: resourceId
  type: string
- description: Repository name of the source image. Specify an image by repository ('hello-world'). This will use the 'latest' tag. Specify an image by tag ('hello-world:latest'). Specify an image by sha256-based ma
  name: sourceImage
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-import-source-schema.json
slug: azure-container-registry-import-source
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: ImportSource
---
