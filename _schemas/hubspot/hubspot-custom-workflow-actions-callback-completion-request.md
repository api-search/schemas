---
description: Request body for completing a single callback
layout: schema
name: CallbackCompletionRequest
properties_list:
- description: The output values to return to the workflow
  name: outputFields
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-custom-workflow-actions-callback-completion-request-schema.json
slug: hubspot-custom-workflow-actions-callback-completion-request
source_filename: hubspot-custom-workflow-actions-callback-completion-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for completing a single callback\",\n  \"properties\": {\n    \"outputFields\": {\n      \"type\": \"object\",\n      \"description\": \"The output values to return to the workflow\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"outputFields\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CallbackCompletionRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-custom-workflow-actions-callback-completion-request-schema.json
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
title: CallbackCompletionRequest
---
