---
description: Request body for batch archiving notes
layout: schema
name: BatchArchiveNotesRequest
properties_list:
- description: Array of note identifiers to archive
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-notes-batch-archive-notes-request-schema.json
slug: hubspot-engagement-notes-batch-archive-notes-request
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for batch archiving notes\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"Array of note identifiers to archive\",\n      \"example\": [\n        {\n          \"id\": \"1024\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Input for reading a single item in a batch\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The note identifier\",\n            \"example\": \"1024\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchArchiveNotesRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-notes-batch-archive-notes-request-schema.json
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
title: BatchArchiveNotesRequest
---
