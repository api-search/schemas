---
description: The api operations properties
layout: schema
name: ApiOperationPropertiesDefinition
properties_list:
- description: The annotation of api operation.
  name: annotation
  type: object
- description: The api reference.
  name: api
  type: object
- description: The description of the api operation.
  name: description
  type: string
- description: The operation inputs definition schema.
  name: inputsDefinition
  type: object
- description: Indicates whether the API operation is notification or not.
  name: isNotification
  type: boolean
- description: Indicates whether the API operation is webhook or not.
  name: isWebhook
  type: boolean
- description: Indicates whether the api operation is pageable.
  name: pageable
  type: boolean
- description: The operation responses definition schemas.
  name: responsesDefinition
  type: object
- description: The summary of the api operation.
  name: summary
  type: string
- description: The trigger type of api operation.
  name: trigger
  type: string
- description: The trigger hint for the api operation.
  name: triggerHint
  type: string
- description: The visibility of the api operation.
  name: visibility
  type: string
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-api-operation-properties-definition-schema.json
slug: azure-logic-apps-api-operation-properties-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-operation-properties-definition-schema.json\",\n  \"title\": \"ApiOperationPropertiesDefinition\",\n  \"description\": \"The api operations properties\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"annotation\": {\n      \"$ref\": \"#/definitions/ApiOperationAnnotation\",\n      \"description\": \"The annotation of api operation.\"\n    },\n    \"api\": {\n      \"$ref\": \"#/definitions/ApiReference\",\n      \"description\": \"The api reference.\"\n    },\n    \"description\": {\n      \"description\": \"The description of the api operation.\",\n      \"type\": \"string\"\n    },\n    \"inputsDefinition\": {\n      \"$ref\": \"#/definitions/SwaggerSchema\",\n      \"description\": \"The operation inputs definition schema.\"\n    },\n    \"isNotification\": {\n      \"description\"\
  : \"Indicates whether the API operation is notification or not.\",\n      \"type\": \"boolean\"\n    },\n    \"isWebhook\": {\n      \"description\": \"Indicates whether the API operation is webhook or not.\",\n      \"type\": \"boolean\"\n    },\n    \"pageable\": {\n      \"description\": \"Indicates whether the api operation is pageable.\",\n      \"type\": \"boolean\"\n    },\n    \"responsesDefinition\": {\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/SwaggerSchema\"\n      },\n      \"description\": \"The operation responses definition schemas.\",\n      \"type\": \"object\"\n    },\n    \"summary\": {\n      \"description\": \"The summary of the api operation.\",\n      \"type\": \"string\"\n    },\n    \"trigger\": {\n      \"description\": \"The trigger type of api operation.\",\n      \"type\": \"string\"\n    },\n    \"triggerHint\": {\n      \"description\": \"The trigger hint for the api operation.\",\n      \"type\": \"string\"\n    },\n    \"visibility\"\
  : {\n      \"description\": \"The visibility of the api operation.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-operation-properties-definition-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: ApiOperationPropertiesDefinition
---
