---
description: A single callback completion input
layout: schema
name: BatchCallbackInput
properties_list:
- description: The unique identifier of the callback
  name: callbackId
  type: string
- description: The output values to return
  name: outputFields
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-custom-workflow-actions-batch-callback-input-schema.json
slug: hubspot-custom-workflow-actions-batch-callback-input
source_filename: hubspot-custom-workflow-actions-batch-callback-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A single callback completion input\",\n  \"properties\": {\n    \"callbackId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the callback\",\n      \"example\": \"500123\"\n    },\n    \"outputFields\": {\n      \"type\": \"object\",\n      \"description\": \"The output values to return\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"callbackId\",\n    \"outputFields\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchCallbackInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-custom-workflow-actions-batch-callback-input-schema.json
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
title: BatchCallbackInput
---
