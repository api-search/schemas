---
description: The api resource metadata.
layout: schema
name: ApiResourceMetadata
properties_list:
- description: The api type.
  name: ApiType
  type: object
- description: The brand color.
  name: brandColor
  type: string
- description: The connection type.
  name: connectionType
  type: string
- description: The connector deployment parameters metadata.
  name: deploymentParameters
  type: object
- description: The hide key.
  name: hideKey
  type: string
- description: The provisioning state.
  name: provisioningState
  type: object
- description: The source.
  name: source
  type: string
- description: The tags.
  name: tags
  type: object
- description: The WSDL import method.
  name: wsdlImportMethod
  type: object
- description: The WSDL service.
  name: wsdlService
  type: object
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-api-resource-metadata-schema.json
slug: azure-logic-apps-api-resource-metadata
source_filename: azure-logic-apps-api-resource-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-resource-metadata-schema.json\",\n  \"title\": \"ApiResourceMetadata\",\n  \"description\": \"The api resource metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApiType\": {\n      \"$ref\": \"#/definitions/ApiType\",\n      \"description\": \"The api type.\"\n    },\n    \"brandColor\": {\n      \"description\": \"The brand color.\",\n      \"type\": \"string\"\n    },\n    \"connectionType\": {\n      \"description\": \"The connection type.\",\n      \"type\": \"string\"\n    },\n    \"deploymentParameters\": {\n      \"$ref\": \"#/definitions/ApiDeploymentParameterMetadataSet\",\n      \"description\": \"The connector deployment parameters metadata.\"\n    },\n    \"hideKey\": {\n      \"description\": \"The hide key.\",\n      \"type\": \"string\"\n    },\n   \
  \ \"provisioningState\": {\n      \"$ref\": \"#/definitions/WorkflowProvisioningState\",\n      \"description\": \"The provisioning state.\"\n    },\n    \"source\": {\n      \"description\": \"The source.\",\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The tags.\",\n      \"type\": \"object\"\n    },\n    \"wsdlImportMethod\": {\n      \"$ref\": \"#/definitions/WsdlImportMethod\",\n      \"description\": \"The WSDL import method.\"\n    },\n    \"wsdlService\": {\n      \"$ref\": \"#/definitions/WsdlService\",\n      \"description\": \"The WSDL service.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-resource-metadata-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: ApiResourceMetadata
---
