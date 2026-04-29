---
description: Request body for batch updating notes
layout: schema
name: BatchUpdateNotesRequest
properties_list:
- description: Array of note updates
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-notes-batch-update-notes-request-schema.json
slug: engagement-notes-batch-update-notes-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-notes-batch-update-notes-request-schema.json\",\n  \"title\": \"BatchUpdateNotesRequest\",\n  \"description\": \"Request body for batch updating notes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"Array of note updates\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Input for updating a single item in a batch\",\n        \"required\": [\n          \"id\",\n          \"properties\"\n        ],\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The note identifier\",\n            \"example\": \"1024\"\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The properties to update\"\
  ,\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        }\n      },\n      \"maxItems\": 100,\n      \"example\": [\n        {\n          \"id\": \"1024\",\n          \"properties\": {\n            \"key\": \"value\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-notes-batch-update-notes-request-schema.json
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
title: BatchUpdateNotesRequest
---
