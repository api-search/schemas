---
description: The API resource properties.
layout: schema
name: ApiResourceProperties
properties_list:
- description: The API definition.
  name: apiDefinitionUrl
  type: string
- description: The api definitions.
  name: apiDefinitions
  type: object
- description: The backend service.
  name: backendService
  type: object
- description: The capabilities.
  name: capabilities
  type: array
- description: The category.
  name: category
  type: object
- description: The connection parameters.
  name: connectionParameters
  type: object
- description: The api general information.
  name: generalInformation
  type: object
- description: The integration service environment reference.
  name: integrationServiceEnvironment
  type: object
- description: The metadata.
  name: metadata
  type: object
- description: The name
  name: name
  type: string
- description: The policies for the API.
  name: policies
  type: object
- description: The provisioning state.
  name: provisioningState
  type: object
- description: The runtime urls.
  name: runtimeUrls
  type: array
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-api-resource-properties-schema.json
slug: azure-logic-apps-api-resource-properties
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: ApiResourceProperties
---
