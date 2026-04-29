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
source_filename: azure-logic-apps-api-resource-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-resource-properties-schema.json\",\n  \"title\": \"ApiResourceProperties\",\n  \"description\": \"The API resource properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiDefinitionUrl\": {\n      \"description\": \"The API definition.\",\n      \"type\": \"string\"\n    },\n    \"apiDefinitions\": {\n      \"$ref\": \"#/definitions/ApiResourceDefinitions\",\n      \"description\": \"The api definitions.\"\n    },\n    \"backendService\": {\n      \"$ref\": \"#/definitions/ApiResourceBackendService\",\n      \"description\": \"The backend service.\"\n    },\n    \"capabilities\": {\n      \"description\": \"The capabilities.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"category\": {\n      \"$ref\": \"#/definitions/ApiTier\"\
  ,\n      \"description\": \"The category.\"\n    },\n    \"connectionParameters\": {\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/Object\"\n      },\n      \"description\": \"The connection parameters.\",\n      \"type\": \"object\"\n    },\n    \"generalInformation\": {\n      \"$ref\": \"#/definitions/ApiResourceGeneralInformation\",\n      \"description\": \"The api general information.\"\n    },\n    \"integrationServiceEnvironment\": {\n      \"$ref\": \"#/definitions/ResourceReference\",\n      \"description\": \"The integration service environment reference.\"\n    },\n    \"metadata\": {\n      \"$ref\": \"#/definitions/ApiResourceMetadata\",\n      \"description\": \"The metadata.\"\n    },\n    \"name\": {\n      \"description\": \"The name\",\n      \"type\": \"string\"\n    },\n    \"policies\": {\n      \"$ref\": \"#/definitions/ApiResourcePolicies\",\n      \"description\": \"The policies for the API.\"\n    },\n    \"provisioningState\": {\n    \
  \  \"$ref\": \"#/definitions/WorkflowProvisioningState\",\n      \"description\": \"The provisioning state.\"\n    },\n    \"runtimeUrls\": {\n      \"description\": \"The runtime urls.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-resource-properties-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: ApiResourceProperties
---
