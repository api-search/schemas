---
description: ImportImageParameters schema from Azure Container Registry API
layout: schema
name: ImportImageParameters
properties_list:
- description: When Force, any existing target tags will be overwritten. When NoForce, any existing target tags will fail the operation before any copying begins.
  name: mode
  type: string
- description: The source of the image.
  name: source
  type: object
- description: List of strings of the form repo[:tag]. When tag is omitted the source will be used (or 'latest' if source tag is also omitted).
  name: targetTags
  type: array
- description: List of strings of repository names to do a manifest only copy. No tag will be created.
  name: untaggedTargetRepositories
  type: array
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-import-image-parameters-schema.json
slug: azure-container-registry-import-image-parameters
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: ImportImageParameters
---
