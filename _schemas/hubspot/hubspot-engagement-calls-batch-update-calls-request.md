---
description: Request body for batch updating calls
layout: schema
name: BatchUpdateCallsRequest
properties_list:
- description: Array of call updates
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-calls-batch-update-calls-request-schema.json
slug: hubspot-engagement-calls-batch-update-calls-request
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for batch updating calls\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"Array of call updates\",\n      \"example\": [\n        {\n          \"id\": \"512\",\n          \"properties\": {\n            \"key\": \"value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Input for updating a single item in a batch\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The call identifier\",\n            \"example\": \"512\"\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The properties to update\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"properties\"\n        ]\n  \
  \    }\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchUpdateCallsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-calls-batch-update-calls-request-schema.json
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
title: BatchUpdateCallsRequest
---
