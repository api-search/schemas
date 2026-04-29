---
description: Represents an error that occurred for a specific item in a batch operation
layout: schema
name: BatchError
properties_list:
- description: Error status code
  name: status
  type: string
- description: Error category
  name: category
  type: string
- description: Human-readable error message
  name: message
  type: string
- description: Additional context about the error
  name: context
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-feature-flags-api-batch-error-schema.json
slug: crm-feature-flags-api-batch-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-batch-error-schema.json\",\n  \"title\": \"BatchError\",\n  \"description\": \"Represents an error that occurred for a specific item in a batch operation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Error status code\",\n      \"example\": \"error\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Error category\",\n      \"example\": \"VALIDATION_ERROR\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\",\n      \"example\": \"Invalid portal ID\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Additional context about the error\",\n      \"additionalProperties\": {\n        \"type\"\
  : \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"category\",\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-batch-error-schema.json
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
title: BatchError
---
