---
description: A serverless function associated with an action
layout: schema
name: ActionFunction
properties_list:
- description: The unique identifier of the function
  name: id
  type: string
- description: The type of function
  name: functionType
  type: string
- description: The JavaScript source code of the function
  name: functionSource
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/custom-workflow-actions-api-action-function-schema.json
slug: custom-workflow-actions-api-action-function
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-action-function-schema.json\",\n  \"title\": \"ActionFunction\",\n  \"description\": \"A serverless function associated with an action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the function\",\n      \"example\": \"500123\"\n    },\n    \"functionType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PRE_ACTION_EXECUTION\",\n        \"PRE_FETCH_OPTIONS\",\n        \"POST_FETCH_OPTIONS\",\n        \"POST_ACTION_EXECUTION\"\n      ],\n      \"description\": \"The type of function\",\n      \"example\": \"PRE_ACTION_EXECUTION\"\n    },\n    \"functionSource\": {\n      \"type\": \"string\",\n      \"description\": \"The JavaScript source code of the function\",\n      \"\
  example\": \"example-value\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"functionType\",\n    \"functionSource\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-action-function-schema.json
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
title: ActionFunction
---
