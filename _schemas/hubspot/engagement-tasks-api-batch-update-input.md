---
description: BatchUpdateInput schema from HubSpot Engagement Tasks API
layout: schema
name: BatchUpdateInput
properties_list:
- description: ''
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-tasks-api-batch-update-input-schema.json
slug: engagement-tasks-api-batch-update-input
source_filename: engagement-tasks-api-batch-update-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-tasks-api-batch-update-input-schema.json\",\n  \"title\": \"BatchUpdateInput\",\n  \"description\": \"BatchUpdateInput schema from HubSpot Engagement Tasks API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"properties\": {\n            \"key\": \"value\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-tasks-api-batch-update-input-schema.json
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
title: BatchUpdateInput
---
