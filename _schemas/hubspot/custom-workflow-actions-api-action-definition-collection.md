---
description: A paginated collection of action definitions
layout: schema
name: ActionDefinitionCollection
properties_list:
- description: List of action definitions
  name: results
  type: array
- description: Pagination information
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/custom-workflow-actions-api-action-definition-collection-schema.json
slug: custom-workflow-actions-api-action-definition-collection
source_filename: custom-workflow-actions-api-action-definition-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-action-definition-collection-schema.json\",\n  \"title\": \"ActionDefinitionCollection\",\n  \"description\": \"A paginated collection of action definitions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"List of action definitions\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A custom workflow action definition\",\n        \"required\": [\n          \"id\",\n          \"revisionId\",\n          \"actionUrl\",\n          \"labels\",\n          \"objectTypes\"\n        ],\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the action definition\",\n            \"example\": \"500123\"\n  \
  \        },\n          \"revisionId\": {\n            \"type\": \"string\",\n            \"description\": \"The current revision identifier\",\n            \"example\": \"500123\"\n          },\n          \"actionUrl\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"The URL that HubSpot will call when the action executes\",\n            \"example\": \"https://app.hubspot.com/contacts/12345\"\n          },\n          \"labels\": {\n            \"$ref\": \"#/components/schemas/ActionLabels\"\n          },\n          \"inputFields\": {\n            \"type\": \"array\",\n            \"description\": \"Input fields that users can configure for the action\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/InputField\"\n            },\n            \"example\": [\n              {\n                \"typeDefinition\": {},\n                \"supportedValueTypes\": [\n                  {}\n                ],\n      \
  \          \"isRequired\": true\n              }\n            ]\n          },\n          \"outputFields\": {\n            \"type\": \"array\",\n            \"description\": \"Output fields that the action returns\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/OutputField\"\n            },\n            \"example\": [\n              {\n                \"typeDefinition\": {}\n              }\n            ]\n          },\n          \"objectTypes\": {\n            \"type\": \"array\",\n            \"description\": \"CRM object types this action can operate on\",\n            \"items\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"CONTACT\",\n                \"COMPANY\",\n                \"DEAL\",\n                \"TICKET\",\n                \"QUOTE\"\n              ]\n            },\n            \"example\": [\n              \"CONTACT\"\n            ]\n          },\n          \"objectRequestOptions\": {\n            \"$ref\"\
  : \"#/components/schemas/ObjectRequestOptions\"\n          },\n          \"published\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the action is published and available for use\",\n            \"example\": true\n          },\n          \"functions\": {\n            \"type\": \"array\",\n            \"description\": \"Functions associated with this action\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/ActionFunctionReference\"\n            },\n            \"example\": [\n              {\n                \"functionType\": \"PRE_ACTION_EXECUTION\",\n                \"id\": \"500123\"\n              }\n            ]\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"revisionId\": \"500123\",\n          \"actionUrl\": \"https://app.hubspot.com/contacts/12345\",\n          \"labels\": {},\n          \"inputFields\": [\n            {\n              \"typeDefinition\": {},\n\
  \              \"supportedValueTypes\": [\n                {}\n              ],\n              \"isRequired\": true\n            }\n          ],\n          \"outputFields\": [\n            {\n              \"typeDefinition\": {}\n            }\n          ],\n          \"objectTypes\": [\n            \"CONTACT\"\n          ],\n          \"objectRequestOptions\": {},\n          \"published\": true,\n          \"functions\": [\n            {\n              \"functionType\": \"PRE_ACTION_EXECUTION\",\n              \"id\": \"500123\"\n            }\n          ]\n        }\n      ]\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor for the next page\"\n            }\n          },\n          \"example\": {\n            \"after\"\
  : \"example-value\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"results\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-action-definition-collection-schema.json
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
title: ActionDefinitionCollection
---
