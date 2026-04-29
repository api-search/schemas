---
description: Input for batch archive operations
layout: schema
name: BatchArchiveInput
properties_list:
- description: Array of author IDs to archive
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-authors-batch-archive-input-schema.json
slug: hubspot-authors-batch-archive-input
source_filename: hubspot-authors-batch-archive-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Input for batch archive operations\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"Array of author IDs to archive\",\n      \"example\": [\n        {\n          \"id\": \"500123\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the author to archive\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchArchiveInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-authors-batch-archive-input-schema.json
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
title: BatchArchiveInput
---
