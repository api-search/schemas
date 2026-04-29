---
description: Error information for a failed callback
layout: schema
name: BatchCallbackError
properties_list:
- description: The callback that failed
  name: callbackId
  type: string
- description: Error message
  name: message
  type: string
- description: Error category
  name: category
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-custom-workflow-actions-batch-callback-error-schema.json
slug: hubspot-custom-workflow-actions-batch-callback-error
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Error information for a failed callback\",\n  \"properties\": {\n    \"callbackId\": {\n      \"type\": \"string\",\n      \"description\": \"The callback that failed\",\n      \"example\": \"500123\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\",\n      \"example\": \"This is an example description.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Error category\",\n      \"example\": \"standard\"\n    }\n  },\n  \"required\": [\n    \"callbackId\",\n    \"message\",\n    \"category\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchCallbackError\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-custom-workflow-actions-batch-callback-error-schema.json
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
title: BatchCallbackError
---
