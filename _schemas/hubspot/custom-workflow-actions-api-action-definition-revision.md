---
description: A revision of an action definition
layout: schema
name: ActionDefinitionRevision
properties_list:
- description: The unique identifier of the revision
  name: revisionId
  type: string
- description: A custom workflow action definition
  name: definition
  type: object
- description: When the revision was created
  name: createdAt
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/custom-workflow-actions-api-action-definition-revision-schema.json
slug: custom-workflow-actions-api-action-definition-revision
source_filename: custom-workflow-actions-api-action-definition-revision-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-action-definition-revision-schema.json\",\n  \"title\": \"ActionDefinitionRevision\",\n  \"description\": \"A revision of an action definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"revisionId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the revision\",\n      \"example\": \"500123\"\n    },\n    \"definition\": {\n      \"type\": \"object\",\n      \"description\": \"A custom workflow action definition\",\n      \"required\": [\n        \"id\",\n        \"revisionId\",\n        \"actionUrl\",\n        \"labels\",\n        \"objectTypes\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the action definition\",\n          \"example\":\
  \ \"500123\"\n        },\n        \"revisionId\": {\n          \"type\": \"string\",\n          \"description\": \"The current revision identifier\",\n          \"example\": \"500123\"\n        },\n        \"actionUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL that HubSpot will call when the action executes\",\n          \"example\": \"https://app.hubspot.com/contacts/12345\"\n        },\n        \"labels\": {\n          \"type\": \"object\",\n          \"description\": \"Human-readable labels for the action\",\n          \"required\": [\n            \"actionName\"\n          ],\n          \"properties\": {\n            \"actionName\": {\n              \"type\": \"string\",\n              \"description\": \"The display name of the action\",\n              \"example\": \"Example Record\"\n            },\n            \"actionDescription\": {\n              \"type\": \"string\",\n              \"description\": \"A description\
  \ of what the action does\",\n              \"example\": \"This is an example description.\"\n            },\n            \"appDisplayName\": {\n              \"type\": \"string\",\n              \"description\": \"The name of the app providing this action\",\n              \"example\": \"Example Record\"\n            },\n            \"actionCardContent\": {\n              \"type\": \"string\",\n              \"description\": \"Content to display on the action card in the workflow editor\",\n              \"example\": \"example-value\"\n            }\n          }\n        },\n        \"inputFields\": {\n          \"type\": \"array\",\n          \"description\": \"Input fields that users can configure for the action\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/InputField\"\n          },\n          \"example\": [\n            {\n              \"typeDefinition\": {},\n              \"supportedValueTypes\": [\n                {}\n              ],\n             \
  \ \"isRequired\": true\n            }\n          ]\n        },\n        \"outputFields\": {\n          \"type\": \"array\",\n          \"description\": \"Output fields that the action returns\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/OutputField\"\n          },\n          \"example\": [\n            {\n              \"typeDefinition\": {}\n            }\n          ]\n        },\n        \"objectTypes\": {\n          \"type\": \"array\",\n          \"description\": \"CRM object types this action can operate on\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"CONTACT\",\n              \"COMPANY\",\n              \"DEAL\",\n              \"TICKET\",\n              \"QUOTE\"\n            ]\n          },\n          \"example\": [\n            \"CONTACT\"\n          ]\n        },\n        \"objectRequestOptions\": {\n          \"type\": \"object\",\n          \"description\": \"Options for requesting CRM object\
  \ data\",\n          \"properties\": {\n            \"properties\": {\n              \"type\": \"array\",\n              \"description\": \"CRM properties to include in the action execution request\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"example\": [\n                \"example-value\"\n              ]\n            }\n          }\n        },\n        \"published\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the action is published and available for use\",\n          \"example\": true\n        },\n        \"functions\": {\n          \"type\": \"array\",\n          \"description\": \"Functions associated with this action\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/ActionFunctionReference\"\n          },\n          \"example\": [\n            {\n              \"functionType\": \"PRE_ACTION_EXECUTION\",\n              \"id\": \"500123\"\n            }\n          ]\n  \
  \      }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the revision was created\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"required\": [\n    \"revisionId\",\n    \"definition\",\n    \"createdAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-action-definition-revision-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: ActionDefinitionRevision
---
