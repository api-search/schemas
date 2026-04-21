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
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: ApiOperationPropertiesDefinition
---
