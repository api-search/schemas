---
description: Response from a batch callback completion operation
layout: schema
name: BatchCallbackResponse
properties_list:
- description: Overall status of the batch operation
  name: status
  type: string
- description: List of errors for failed callbacks
  name: errors
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/custom-workflow-actions-api-batch-callback-response-schema.json
slug: custom-workflow-actions-api-batch-callback-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-batch-callback-response-schema.json\",\n  \"title\": \"BatchCallbackResponse\",\n  \"description\": \"Response from a batch callback completion operation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"COMPLETE\",\n        \"PARTIAL\"\n      ],\n      \"description\": \"Overall status of the batch operation\",\n      \"example\": \"COMPLETE\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of errors for failed callbacks\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Error information for a failed callback\",\n        \"required\": [\n          \"callbackId\",\n          \"message\",\n          \"category\"\n        ],\n        \"properties\"\
  : {\n          \"callbackId\": {\n            \"type\": \"string\",\n            \"description\": \"The callback that failed\",\n            \"example\": \"500123\"\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"Error message\",\n            \"example\": \"This is an example description.\"\n          },\n          \"category\": {\n            \"type\": \"string\",\n            \"description\": \"Error category\",\n            \"example\": \"standard\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"callbackId\": \"500123\",\n          \"message\": \"This is an example description.\",\n          \"category\": \"standard\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-batch-callback-response-schema.json
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
title: BatchCallbackResponse
---
