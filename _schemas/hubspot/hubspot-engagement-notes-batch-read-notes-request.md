---
description: Request body for batch reading notes
layout: schema
name: BatchReadNotesRequest
properties_list:
- description: Array of note identifiers
  name: inputs
  type: array
- description: Properties to return
  name: properties
  type: array
- description: Properties to return with history
  name: propertiesWithHistory
  type: array
- description: The property to use as the identifier
  name: idProperty
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-notes-batch-read-notes-request-schema.json
slug: hubspot-engagement-notes-batch-read-notes-request
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for batch reading notes\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"Array of note identifiers\",\n      \"example\": [\n        {\n          \"id\": \"1024\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Input for reading a single item in a batch\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The note identifier\",\n            \"example\": \"1024\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ]\n      }\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"Properties to return\",\n      \"example\": [\n        \"example-value\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"propertiesWithHistory\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Properties to return with history\",\n      \"example\": [\n        \"example-value\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"idProperty\": {\n      \"type\": \"string\",\n      \"description\": \"The property to use as the identifier\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchReadNotesRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-notes-batch-read-notes-request-schema.json
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
title: BatchReadNotesRequest
---
