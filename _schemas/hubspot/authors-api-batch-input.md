---
description: Input for batch update operations
layout: schema
name: BatchInput
properties_list:
- description: Array of items to process
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/authors-api-batch-input-schema.json
slug: authors-api-batch-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-batch-input-schema.json\",\n  \"title\": \"BatchInput\",\n  \"description\": \"Input for batch update operations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Single item in a batch update operation\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the author to update\",\n            \"example\": \"500123\"\n          },\n          \"properties\": {\n            \"$ref\": \"#/components/schemas/BlogAuthorInput\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ]\n      },\n      \"description\": \"Array of items to process\",\n      \"example\": [\n        {\n          \"\
  id\": \"500123\",\n          \"properties\": {}\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-batch-input-schema.json
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
title: BatchInput
---
