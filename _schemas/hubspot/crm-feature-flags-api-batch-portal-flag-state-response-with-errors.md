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
schema_file: json-schema/crm-feature-flags-api-batch-portal-flag-state-response-with-errors-schema.json
slug: crm-feature-flags-api-batch-portal-flag-state-response-with-errors
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-batch-portal-flag-state-response-with-errors-schema.json\",\n  \"title\": \"BatchPortalFlagStateResponseWithErrors\",\n  \"description\": \"Response for batch operations that had some failures\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The overall status of the batch operation\",\n      \"enum\": [\n        \"COMPLETE\",\n        \"PENDING\"\n      ],\n      \"example\": \"COMPLETE\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"List of portal flag states that were successfully affected\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents the flag state override for a specific portal (account)\",\n        \"required\": [\n          \"\
  appId\",\n          \"flagName\",\n          \"portalId\",\n          \"flagState\"\n        ],\n        \"properties\": {\n          \"appId\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"description\": \"The unique identifier for the HubSpot application\",\n            \"example\": 12345678\n          },\n          \"flagName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the feature flag\",\n            \"example\": \"new-dashboard-feature\"\n          },\n          \"portalId\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"description\": \"The unique identifier for the HubSpot portal (account)\",\n            \"example\": 98765432\n          },\n          \"flagState\": {\n            \"$ref\": \"#/components/schemas/FlagState\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"appId\": 12345678,\n          \"flagName\": \"new-dashboard-feature\"\
  ,\n          \"portalId\": 98765432,\n          \"flagState\": {}\n        }\n      ]\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of errors that occurred during the batch operation\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents an error that occurred for a specific item in a batch operation\",\n        \"required\": [\n          \"status\",\n          \"category\",\n          \"message\"\n        ],\n        \"properties\": {\n          \"status\": {\n            \"type\": \"string\",\n            \"description\": \"Error status code\",\n            \"example\": \"error\"\n          },\n          \"category\": {\n            \"type\": \"string\",\n            \"description\": \"Error category\",\n            \"example\": \"VALIDATION_ERROR\"\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"Human-readable error message\",\n            \"example\"\
  : \"Invalid portal ID\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"description\": \"Additional context about the error\",\n            \"additionalProperties\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"status\": \"error\",\n          \"category\": \"VALIDATION_ERROR\",\n          \"message\": \"Invalid portal ID\",\n          \"context\": {\n            \"key\": \"value\"\n          }\n        }\n      ]\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the batch operation started\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"\
  date-time\",\n      \"description\": \"Timestamp when the batch operation completed\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"results\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-batch-portal-flag-state-response-with-errors-schema.json
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
