---
description: A reference to a function associated with an action
layout: schema
name: ActionFunctionReference
properties_list:
- description: The type of function
  name: functionType
  type: string
- description: The unique identifier of the function
  name: id
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-custom-workflow-actions-action-function-reference-schema.json
slug: hubspot-custom-workflow-actions-action-function-reference
source_filename: hubspot-custom-workflow-actions-action-function-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A reference to a function associated with an action\",\n  \"properties\": {\n    \"functionType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of function\",\n      \"example\": \"PRE_ACTION_EXECUTION\",\n      \"enum\": [\n        \"PRE_ACTION_EXECUTION\",\n        \"PRE_FETCH_OPTIONS\",\n        \"POST_FETCH_OPTIONS\",\n        \"POST_ACTION_EXECUTION\"\n      ]\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the function\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"functionType\",\n    \"id\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActionFunctionReference\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-custom-workflow-actions-action-function-reference-schema.json
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
title: ActionFunctionReference
---
