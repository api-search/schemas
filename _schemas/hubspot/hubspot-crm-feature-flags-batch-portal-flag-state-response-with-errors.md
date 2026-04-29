---
description: Response for batch operations that had some failures
layout: schema
name: BatchPortalFlagStateResponseWithErrors
properties_list:
- description: The overall status of the batch operation
  name: status
  type: string
- description: List of portal flag states that were successfully affected
  name: results
  type: array
- description: List of errors that occurred during the batch operation
  name: errors
  type: array
- description: Timestamp when the batch operation started
  name: startedAt
  type: string
- description: Timestamp when the batch operation completed
  name: completedAt
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-feature-flags-batch-portal-flag-state-response-with-errors-schema.json
slug: hubspot-crm-feature-flags-batch-portal-flag-state-response-with-errors
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response for batch operations that had some failures\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The overall status of the batch operation\",\n      \"example\": \"COMPLETE\",\n      \"enum\": [\n        \"COMPLETE\",\n        \"PENDING\"\n      ]\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"List of portal flag states that were successfully affected\",\n      \"example\": [\n        {\n          \"appId\": 12345678,\n          \"flagName\": \"new-dashboard-feature\",\n          \"portalId\": 98765432,\n          \"flagState\": {}\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents the flag state override for a specific portal (account)\",\n        \"properties\": {\n          \"appId\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique identifier for\
  \ the HubSpot application\",\n            \"format\": \"int64\",\n            \"example\": 12345678\n          },\n          \"flagName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the feature flag\",\n            \"example\": \"new-dashboard-feature\"\n          },\n          \"portalId\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique identifier for the HubSpot portal (account)\",\n            \"format\": \"int64\",\n            \"example\": 98765432\n          },\n          \"flagState\": {\n            \"type\": \"string\",\n            \"description\": \"The state of a feature flag\",\n            \"example\": \"ON\",\n            \"enum\": [\n              \"ON\",\n              \"OFF\",\n              \"ABSENT\"\n            ]\n          }\n        },\n        \"required\": [\n          \"appId\",\n          \"flagName\",\n          \"portalId\",\n          \"flagState\"\n        ]\n      }\n    },\n    \"\
  errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of errors that occurred during the batch operation\",\n      \"example\": [\n        {\n          \"status\": \"error\",\n          \"category\": \"VALIDATION_ERROR\",\n          \"message\": \"Invalid portal ID\",\n          \"context\": {\n            \"key\": \"value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents an error that occurred for a specific item in a batch operation\",\n        \"properties\": {\n          \"status\": {\n            \"type\": \"string\",\n            \"description\": \"Error status code\",\n            \"example\": \"error\"\n          },\n          \"category\": {\n            \"type\": \"string\",\n            \"description\": \"Error category\",\n            \"example\": \"VALIDATION_ERROR\"\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"Human-readable\
  \ error message\",\n            \"example\": \"Invalid portal ID\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"description\": \"Additional context about the error\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        },\n        \"required\": [\n          \"status\",\n          \"category\",\n          \"message\"\n        ]\n      }\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the batch operation started\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the batch operation completed\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"results\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\"\
  : \"BatchPortalFlagStateResponseWithErrors\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-feature-flags-batch-portal-flag-state-response-with-errors-schema.json
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
title: BatchPortalFlagStateResponseWithErrors
---
