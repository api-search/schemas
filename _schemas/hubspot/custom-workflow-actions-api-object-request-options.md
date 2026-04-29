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
schema_file: json-schema/custom-workflow-actions-api-object-request-options-schema.json
slug: custom-workflow-actions-api-object-request-options
source_filename: custom-workflow-actions-api-object-request-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-object-request-options-schema.json\",\n  \"title\": \"ObjectRequestOptions\",\n  \"description\": \"Options for requesting CRM object data\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"CRM properties to include in the action execution request\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"example-value\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-object-request-options-schema.json
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
