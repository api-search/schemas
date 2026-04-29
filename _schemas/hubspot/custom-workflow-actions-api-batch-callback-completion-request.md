---
description: Request body for completing multiple callbacks
layout: schema
name: BatchCallbackCompletionRequest
properties_list:
- description: List of callbacks to complete
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/custom-workflow-actions-api-batch-callback-completion-request-schema.json
slug: custom-workflow-actions-api-batch-callback-completion-request
source_filename: custom-workflow-actions-api-batch-callback-completion-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-batch-callback-completion-request-schema.json\",\n  \"title\": \"BatchCallbackCompletionRequest\",\n  \"description\": \"Request body for completing multiple callbacks\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"List of callbacks to complete\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A single callback completion input\",\n        \"required\": [\n          \"callbackId\",\n          \"outputFields\"\n        ],\n        \"properties\": {\n          \"callbackId\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the callback\",\n            \"example\": \"500123\"\n          },\n          \"outputFields\": {\n            \"\
  type\": \"object\",\n            \"description\": \"The output values to return\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"callbackId\": \"500123\",\n          \"outputFields\": {\n            \"key\": \"value\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-batch-callback-completion-request-schema.json
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
title: BatchCallbackCompletionRequest
---
