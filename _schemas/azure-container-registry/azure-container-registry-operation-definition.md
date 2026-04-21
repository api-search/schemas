---
description: The definition of a container registry operation.
layout: schema
name: OperationDefinition
properties_list:
- description: The display information for the container registry operation.
  name: display
  type: object
- description: 'Operation name: {provider}/{resource}/{operation}.'
  name: name
  type: string
- description: The origin information of the container registry operation.
  name: origin
  type: string
- description: The properties information for the container registry operation.
  name: properties
  type: object
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-operation-definition-schema.json
slug: azure-container-registry-operation-definition
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: OperationDefinition
---
