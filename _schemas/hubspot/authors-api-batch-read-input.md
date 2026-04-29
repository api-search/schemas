---
description: Input for batch read operations
layout: schema
name: BatchReadInput
properties_list:
- description: Array of author IDs to retrieve
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/authors-api-batch-read-input-schema.json
slug: authors-api-batch-read-input
source_filename: authors-api-batch-read-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-batch-read-input-schema.json\",\n  \"title\": \"BatchReadInput\",\n  \"description\": \"Input for batch read operations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the author to read\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ]\n      },\n      \"description\": \"Array of author IDs to retrieve\",\n      \"example\": [\n        {\n          \"id\": \"500123\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-batch-read-input-schema.json
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
title: BatchReadInput
---
