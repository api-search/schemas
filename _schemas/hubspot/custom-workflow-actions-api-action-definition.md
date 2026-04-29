---
description: A custom workflow action definition
layout: schema
name: ActionDefinition
properties_list:
- description: The unique identifier of the action definition
  name: id
  type: string
- description: The current revision identifier
  name: revisionId
  type: string
- description: The URL that HubSpot will call when the action executes
  name: actionUrl
  type: string
- description: Human-readable labels for the action
  name: labels
  type: object
- description: Input fields that users can configure for the action
  name: inputFields
  type: array
- description: Output fields that the action returns
  name: outputFields
  type: array
- description: CRM object types this action can operate on
  name: objectTypes
  type: array
- description: Options for requesting CRM object data
  name: objectRequestOptions
  type: object
- description: Whether the action is published and available for use
  name: published
  type: boolean
- description: Functions associated with this action
  name: functions
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/custom-workflow-actions-api-action-definition-schema.json
slug: custom-workflow-actions-api-action-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-action-definition-schema.json\",\n  \"title\": \"ActionDefinition\",\n  \"description\": \"A custom workflow action definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the action definition\",\n      \"example\": \"500123\"\n    },\n    \"revisionId\": {\n      \"type\": \"string\",\n      \"description\": \"The current revision identifier\",\n      \"example\": \"500123\"\n    },\n    \"actionUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL that HubSpot will call when the action executes\",\n      \"example\": \"https://app.hubspot.com/contacts/12345\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Human-readable labels for the action\",\n      \"required\": [\n        \"actionName\"\n      ],\n      \"properties\": {\n        \"actionName\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the action\",\n          \"example\": \"Example Record\"\n        },\n        \"actionDescription\": {\n          \"type\": \"string\",\n          \"description\": \"A description of what the action does\",\n          \"example\": \"This is an example description.\"\n        },\n        \"appDisplayName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the app providing this action\",\n          \"example\": \"Example Record\"\n        },\n        \"actionCardContent\": {\n          \"type\": \"string\",\n          \"description\": \"Content to display on the action card in the workflow editor\",\n          \"example\": \"example-value\"\n        }\n      }\n    },\n    \"inputFields\": {\n      \"type\": \"array\",\n      \"\
  description\": \"Input fields that users can configure for the action\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"An input field for the action\",\n        \"required\": [\n          \"typeDefinition\",\n          \"supportedValueTypes\"\n        ],\n        \"properties\": {\n          \"typeDefinition\": {\n            \"$ref\": \"#/components/schemas/FieldTypeDefinition\"\n          },\n          \"supportedValueTypes\": {\n            \"type\": \"array\",\n            \"description\": \"The types of values that can be provided for this field\",\n            \"items\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"STATIC_VALUE\",\n                \"OBJECT_PROPERTY\",\n                \"OUTPUT_FROM_PREVIOUS_ACTION\"\n              ]\n            },\n            \"example\": [\n              \"STATIC_VALUE\"\n            ]\n          },\n          \"isRequired\": {\n            \"type\": \"boolean\",\n      \
  \      \"description\": \"Whether this field is required\",\n            \"example\": true\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"typeDefinition\": {},\n          \"supportedValueTypes\": [\n            {}\n          ],\n          \"isRequired\": true\n        }\n      ]\n    },\n    \"outputFields\": {\n      \"type\": \"array\",\n      \"description\": \"Output fields that the action returns\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"An output field returned by the action\",\n        \"required\": [\n          \"typeDefinition\"\n        ],\n        \"properties\": {\n          \"typeDefinition\": {\n            \"$ref\": \"#/components/schemas/FieldTypeDefinition\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"typeDefinition\": {}\n        }\n      ]\n    },\n    \"objectTypes\": {\n      \"type\": \"array\",\n      \"description\": \"CRM object types this action can operate\
  \ on\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"CONTACT\",\n          \"COMPANY\",\n          \"DEAL\",\n          \"TICKET\",\n          \"QUOTE\"\n        ]\n      },\n      \"example\": [\n        \"CONTACT\"\n      ]\n    },\n    \"objectRequestOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Options for requesting CRM object data\",\n      \"properties\": {\n        \"properties\": {\n          \"type\": \"array\",\n          \"description\": \"CRM properties to include in the action execution request\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"example\": [\n            \"example-value\"\n          ]\n        }\n      }\n    },\n    \"published\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the action is published and available for use\",\n      \"example\": true\n    },\n    \"functions\": {\n      \"type\": \"array\",\n      \"description\": \"Functions\
  \ associated with this action\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A reference to a function associated with an action\",\n        \"required\": [\n          \"functionType\",\n          \"id\"\n        ],\n        \"properties\": {\n          \"functionType\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"PRE_ACTION_EXECUTION\",\n              \"PRE_FETCH_OPTIONS\",\n              \"POST_FETCH_OPTIONS\",\n              \"POST_ACTION_EXECUTION\"\n            ],\n            \"description\": \"The type of function\",\n            \"example\": \"PRE_ACTION_EXECUTION\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the function\",\n            \"example\": \"500123\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"functionType\": \"PRE_ACTION_EXECUTION\",\n          \"id\": \"500123\"\n        }\n    \
  \  ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"revisionId\",\n    \"actionUrl\",\n    \"labels\",\n    \"objectTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-action-definition-schema.json
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
title: ActionDefinition
---
