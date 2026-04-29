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
schema_file: json-schema/hubspot-crm-feature-flags-batch-portal-flag-state-response-schema.json
slug: hubspot-crm-feature-flags-batch-portal-flag-state-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response for successful batch portal flag state operations\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The overall status of the batch operation\",\n      \"example\": \"COMPLETE\",\n      \"enum\": [\n        \"COMPLETE\",\n        \"PENDING\"\n      ]\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"List of portal flag states that were successfully affected\",\n      \"example\": [\n        {\n          \"appId\": 12345678,\n          \"flagName\": \"new-dashboard-feature\",\n          \"portalId\": 98765432,\n          \"flagState\": {}\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents the flag state override for a specific portal (account)\",\n        \"properties\": {\n          \"appId\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique identifier\
  \ for the HubSpot application\",\n            \"format\": \"int64\",\n            \"example\": 12345678\n          },\n          \"flagName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the feature flag\",\n            \"example\": \"new-dashboard-feature\"\n          },\n          \"portalId\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique identifier for the HubSpot portal (account)\",\n            \"format\": \"int64\",\n            \"example\": 98765432\n          },\n          \"flagState\": {\n            \"type\": \"string\",\n            \"description\": \"The state of a feature flag\",\n            \"example\": \"ON\",\n            \"enum\": [\n              \"ON\",\n              \"OFF\",\n              \"ABSENT\"\n            ]\n          }\n        },\n        \"required\": [\n          \"appId\",\n          \"flagName\",\n          \"portalId\",\n          \"flagState\"\n        ]\n      }\n    },\n  \
  \  \"startedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the batch operation started\",\n      \"format\": \"date-time\",\n      \"example\": \"2024-01-15T10:30:00Z\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the batch operation completed\",\n      \"format\": \"date-time\",\n      \"example\": \"2024-01-15T10:30:01Z\"\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"results\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchPortalFlagStateResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-feature-flags-batch-portal-flag-state-response-schema.json
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
