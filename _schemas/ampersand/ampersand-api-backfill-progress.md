---
description: BackfillProgress schema from Ampersand API
layout: schema
name: BackfillProgress
properties_list:
- description: The installation ID.
  name: installationId
  type: string
- description: The object being synced (e.g., contact, account).
  name: objectName
  type: string
- description: The ID of the backfill operation.
  name: operationId
  type: string
- description: The number of records processed so far. Updates as more records are read during the backfill.
  name: recordsProcessed
  type: integer
- description: The estimated total number of records to process. Only present for Salesforce and HubSpot; other connectors omit this field.
  name: recordsEstimatedTotal
  type: integer
- description: When the backfill operation started.
  name: createTime
  type: string
- description: When progress was last updated.
  name: updateTime
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-backfill-progress-schema.json
slug: ampersand-api-backfill-progress
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-backfill-progress-schema.json\",\n  \"title\": \"BackfillProgress\",\n  \"description\": \"BackfillProgress schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"installationId\": {\n      \"type\": \"string\",\n      \"description\": \"The installation ID.\"\n    },\n    \"objectName\": {\n      \"type\": \"string\",\n      \"description\": \"The object being synced (e.g., contact, account).\"\n    },\n    \"operationId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the backfill operation.\"\n    },\n    \"recordsProcessed\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of records processed so far. Updates as more records are read during the backfill.\",\n      \"example\": 1250\n    },\n    \"recordsEstimatedTotal\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"The estimated total number of records to process. Only present for Salesforce and HubSpot; other connectors omit this field.\",\n      \"example\": 5000\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the backfill operation started.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When progress was last updated.\"\n    }\n  },\n  \"required\": [\n    \"installationId\",\n    \"objectName\",\n    \"operationId\",\n    \"recordsProcessed\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-backfill-progress-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: BackfillProgress
---
