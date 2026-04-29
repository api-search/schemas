---
description: A collection of action functions
layout: schema
name: ActionFunctionCollection
properties_list:
- description: List of action functions
  name: results
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/custom-workflow-actions-api-action-function-collection-schema.json
slug: custom-workflow-actions-api-action-function-collection
source_filename: custom-workflow-actions-api-action-function-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-action-function-collection-schema.json\",\n  \"title\": \"ActionFunctionCollection\",\n  \"description\": \"A collection of action functions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"List of action functions\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A serverless function associated with an action\",\n        \"required\": [\n          \"id\",\n          \"functionType\",\n          \"functionSource\"\n        ],\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the function\",\n            \"example\": \"500123\"\n          },\n          \"functionType\": {\n            \"type\"\
  : \"string\",\n            \"enum\": [\n              \"PRE_ACTION_EXECUTION\",\n              \"PRE_FETCH_OPTIONS\",\n              \"POST_FETCH_OPTIONS\",\n              \"POST_ACTION_EXECUTION\"\n            ],\n            \"description\": \"The type of function\",\n            \"example\": \"PRE_ACTION_EXECUTION\"\n          },\n          \"functionSource\": {\n            \"type\": \"string\",\n            \"description\": \"The JavaScript source code of the function\",\n            \"example\": \"example-value\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"functionType\": \"PRE_ACTION_EXECUTION\",\n          \"functionSource\": \"example-value\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"results\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-action-function-collection-schema.json
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
title: ActionFunctionCollection
---
