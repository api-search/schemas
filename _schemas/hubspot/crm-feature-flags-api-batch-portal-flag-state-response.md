---
description: Response for successful batch portal flag state operations
layout: schema
name: BatchPortalFlagStateResponse
properties_list:
- description: The overall status of the batch operation
  name: status
  type: string
- description: List of portal flag states that were successfully affected
  name: results
  type: array
- description: Timestamp when the batch operation started
  name: startedAt
  type: string
- description: Timestamp when the batch operation completed
  name: completedAt
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-feature-flags-api-batch-portal-flag-state-response-schema.json
slug: crm-feature-flags-api-batch-portal-flag-state-response
source_filename: crm-feature-flags-api-batch-portal-flag-state-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-batch-portal-flag-state-response-schema.json\",\n  \"title\": \"BatchPortalFlagStateResponse\",\n  \"description\": \"Response for successful batch portal flag state operations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The overall status of the batch operation\",\n      \"enum\": [\n        \"COMPLETE\",\n        \"PENDING\"\n      ],\n      \"example\": \"COMPLETE\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"List of portal flag states that were successfully affected\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents the flag state override for a specific portal (account)\",\n        \"required\": [\n          \"appId\",\n      \
  \    \"flagName\",\n          \"portalId\",\n          \"flagState\"\n        ],\n        \"properties\": {\n          \"appId\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"description\": \"The unique identifier for the HubSpot application\",\n            \"example\": 12345678\n          },\n          \"flagName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the feature flag\",\n            \"example\": \"new-dashboard-feature\"\n          },\n          \"portalId\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"description\": \"The unique identifier for the HubSpot portal (account)\",\n            \"example\": 98765432\n          },\n          \"flagState\": {\n            \"$ref\": \"#/components/schemas/FlagState\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"appId\": 12345678,\n          \"flagName\": \"new-dashboard-feature\"\
  ,\n          \"portalId\": 98765432,\n          \"flagState\": {}\n        }\n      ]\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the batch operation started\",\n      \"example\": \"2024-01-15T10:30:00Z\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the batch operation completed\",\n      \"example\": \"2024-01-15T10:30:01Z\"\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"results\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-batch-portal-flag-state-response-schema.json
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
title: BatchPortalFlagStateResponse
---
