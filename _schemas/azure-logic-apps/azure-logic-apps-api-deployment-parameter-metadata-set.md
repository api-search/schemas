---
description: The API deployment parameters metadata.
layout: schema
name: ApiDeploymentParameterMetadataSet
properties_list:
- description: The package content link parameter.
  name: packageContentLink
  type: object
- description: The package content link parameter.
  name: redisCacheConnectionString
  type: object
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-api-deployment-parameter-metadata-set-schema.json
slug: azure-logic-apps-api-deployment-parameter-metadata-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-deployment-parameter-metadata-set-schema.json\",\n  \"title\": \"ApiDeploymentParameterMetadataSet\",\n  \"description\": \"The API deployment parameters metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"packageContentLink\": {\n      \"$ref\": \"#/definitions/ApiDeploymentParameterMetadata\",\n      \"description\": \"The package content link parameter.\"\n    },\n    \"redisCacheConnectionString\": {\n      \"$ref\": \"#/definitions/ApiDeploymentParameterMetadata\",\n      \"description\": \"The package content link parameter.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-deployment-parameter-metadata-set-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: ApiDeploymentParameterMetadataSet
---
