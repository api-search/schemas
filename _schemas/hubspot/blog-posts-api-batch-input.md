---
description: Input for batch archive operations
layout: schema
name: BatchInput
properties_list:
- description: Array of items to process
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/blog-posts-api-batch-input-schema.json
slug: blog-posts-api-batch-input
source_filename: blog-posts-api-batch-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-batch-input-schema.json\",\n  \"title\": \"BatchInput\",\n  \"description\": \"Input for batch archive operations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Single item in a batch archive operation\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the post to process\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ]\n      },\n      \"description\": \"Array of items to process\",\n      \"example\": [\n        {\n          \"id\": \"500123\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-batch-input-schema.json
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
