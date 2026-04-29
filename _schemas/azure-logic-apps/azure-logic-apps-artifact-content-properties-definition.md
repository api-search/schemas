---
description: The artifact content properties definition.
layout: schema
name: ArtifactContentPropertiesDefinition
properties_list:
- description: ''
  name: content
  type: object
- description: The content link.
  name: contentLink
  type: object
- description: The content type.
  name: contentType
  type: string
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-artifact-content-properties-definition-schema.json
slug: azure-logic-apps-artifact-content-properties-definition
source_filename: azure-logic-apps-artifact-content-properties-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-artifact-content-properties-definition-schema.json\",\n  \"title\": \"ArtifactContentPropertiesDefinition\",\n  \"description\": \"The artifact content properties definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {},\n    \"contentLink\": {\n      \"$ref\": \"#/definitions/ContentLink\",\n      \"description\": \"The content link.\"\n    },\n    \"contentType\": {\n      \"description\": \"The content type.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-artifact-content-properties-definition-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: ArtifactContentPropertiesDefinition
---
