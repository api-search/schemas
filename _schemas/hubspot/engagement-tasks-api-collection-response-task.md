---
description: CollectionResponseTask schema from HubSpot Engagement Tasks API
layout: schema
name: CollectionResponseTask
properties_list:
- description: ''
  name: results
  type: array
- description: ''
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-tasks-api-collection-response-task-schema.json
slug: engagement-tasks-api-collection-response-task
source_filename: engagement-tasks-api-collection-response-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-tasks-api-collection-response-task-schema.json\",\n  \"title\": \"CollectionResponseTask\",\n  \"description\": \"CollectionResponseTask schema from HubSpot Engagement Tasks API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A HubSpot task engagement record.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the task.\",\n            \"example\": \"500123\"\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The task's properties as key-value pairs.\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\
  \n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"updatedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"archived\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"associations\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"$ref\": \"#/components/schemas/CollectionResponseAssociation\"\n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"properties\": {\n            \"key\": \"value\"\n       \
  \   },\n          \"createdAt\": \"2025-03-15T14:30:00Z\",\n          \"updatedAt\": \"2025-03-15T14:30:00Z\",\n          \"archived\": true,\n          \"associations\": {\n            \"key\": \"value\"\n          }\n        }\n      ]\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\"\n            }\n          },\n          \"example\": {\n            \"after\": \"example-value\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-tasks-api-collection-response-task-schema.json
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
title: CollectionResponseTask
---
