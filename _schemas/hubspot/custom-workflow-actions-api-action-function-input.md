---
description: Input for creating or updating a function
layout: schema
name: ActionFunctionInput
properties_list:
- description: The JavaScript source code of the function
  name: functionSource
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/custom-workflow-actions-api-action-function-input-schema.json
slug: custom-workflow-actions-api-action-function-input
source_filename: custom-workflow-actions-api-action-function-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-action-function-input-schema.json\",\n  \"title\": \"ActionFunctionInput\",\n  \"description\": \"Input for creating or updating a function\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"functionSource\": {\n      \"type\": \"string\",\n      \"description\": \"The JavaScript source code of the function\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"required\": [\n    \"functionSource\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-action-function-input-schema.json
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
title: ActionFunctionInput
---
