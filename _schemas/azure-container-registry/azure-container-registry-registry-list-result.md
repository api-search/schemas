---
description: The result of a request to list container registries.
layout: schema
name: RegistryListResult
properties_list:
- description: The URI that can be used to request the next list of container registries.
  name: nextLink
  type: string
- description: The list of container registries. Since this list may be incomplete, the nextLink field should be used to request the next list of container registries.
  name: value
  type: array
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-registry-list-result-schema.json
slug: azure-container-registry-registry-list-result
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: RegistryListResult
---
