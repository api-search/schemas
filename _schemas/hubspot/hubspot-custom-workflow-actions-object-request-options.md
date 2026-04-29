---
description: Options for requesting CRM object data
layout: schema
name: ObjectRequestOptions
properties_list:
- description: CRM properties to include in the action execution request
  name: properties
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-custom-workflow-actions-object-request-options-schema.json
slug: hubspot-custom-workflow-actions-object-request-options
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Options for requesting CRM object data\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"CRM properties to include in the action execution request\",\n      \"example\": [\n        \"example-value\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectRequestOptions\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-custom-workflow-actions-object-request-options-schema.json
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
title: ObjectRequestOptions
---
