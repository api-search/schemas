---
description: Response for batch note operations
layout: schema
name: BatchNotesResponse
properties_list:
- description: The status of the batch operation
  name: status
  type: string
- description: The results of the batch operation
  name: results
  type: array
- description: When the batch was requested
  name: requestedAt
  type: string
- description: When the batch processing started
  name: startedAt
  type: string
- description: When the batch processing completed
  name: completedAt
  type: string
- description: Any errors that occurred during batch processing
  name: errors
  type: array
- description: ''
  name: links
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-notes-batch-notes-response-schema.json
slug: hubspot-engagement-notes-batch-notes-response
source_filename: hubspot-engagement-notes-batch-notes-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response for batch note operations\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the batch operation\",\n      \"example\": \"COMPLETE\",\n      \"enum\": [\n        \"PENDING\",\n        \"PROCESSING\",\n        \"CANCELED\",\n        \"COMPLETE\"\n      ]\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"The results of the batch operation\",\n      \"example\": [\n        {\n          \"id\": \"1024\",\n          \"properties\": {\n            \"hs_note_body\": \"Met with client to discuss Q1 goals. They are interested in expanding their subscription.\",\n            \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\",\n            \"hubspot_owner_id\": \"12345\"\n          },\n          \"propertiesWithHistory\": {\n            \"key\": \"value\"\n          },\n          \"createdAt\": \"2024-01-15T10:30:00.000Z\",\n          \"updatedAt\"\
  : \"2024-01-15T11:00:00.000Z\",\n          \"archived\": false,\n          \"archivedAt\": \"2025-03-15T14:30:00Z\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents a note engagement in the CRM\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the note\",\n            \"example\": \"1024\"\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The note properties\",\n            \"example\": {\n              \"hs_note_body\": \"Met with client to discuss Q1 goals. They are interested in expanding their subscription.\",\n              \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\",\n              \"hubspot_owner_id\": \"12345\"\n            }\n          },\n          \"propertiesWithHistory\": {\n            \"type\": \"object\",\n            \"description\": \"Properties with their\
  \ change history\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"description\": \"When the note was created\",\n            \"format\": \"date-time\",\n            \"example\": \"2024-01-15T10:30:00.000Z\"\n          },\n          \"updatedAt\": {\n            \"type\": \"string\",\n            \"description\": \"When the note was last updated\",\n            \"format\": \"date-time\",\n            \"example\": \"2024-01-15T11:00:00.000Z\"\n          },\n          \"archived\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the note is archived\",\n            \"example\": false\n          },\n          \"archivedAt\": {\n            \"type\": \"string\",\n            \"description\": \"When the note was archived (if archived)\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          }\n\
  \        },\n        \"required\": [\n          \"id\",\n          \"properties\",\n          \"createdAt\",\n          \"updatedAt\",\n          \"archived\"\n        ]\n      }\n    },\n    \"requestedAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the batch was requested\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the batch processing started\",\n      \"format\": \"date-time\",\n      \"example\": \"2024-01-15T10:30:00.000Z\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the batch processing completed\",\n      \"format\": \"date-time\",\n      \"example\": \"2024-01-15T10:30:05.000Z\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Any errors that occurred during batch processing\",\n      \"example\": [\n        {\n          \"status\": \"error\",\n       \
  \   \"category\": \"VALIDATION_ERROR\",\n          \"message\": \"Property value is invalid\",\n          \"context\": {\n            \"key\": \"value\"\n          },\n          \"errors\": [\n            {}\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Error information for a batch operation item\",\n        \"properties\": {\n          \"status\": {\n            \"type\": \"string\",\n            \"description\": \"The error status\",\n            \"example\": \"error\"\n          },\n          \"category\": {\n            \"type\": \"string\",\n            \"description\": \"The error category\",\n            \"example\": \"VALIDATION_ERROR\"\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"The error message\",\n            \"example\": \"Property value is invalid\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"example\"\
  : {\n              \"key\": \"value\"\n            }\n          },\n          \"errors\": {\n            \"type\": \"array\",\n            \"example\": [\n              {\n                \"message\": \"This is an example description.\",\n                \"code\": \"example-value\",\n                \"in\": \"example-value\",\n                \"subCategory\": \"standard\",\n                \"context\": {\n                  \"key\": \"value\"\n                }\n              }\n            ],\n            \"items\": {\n              \"type\": \"object\",\n              \"description\": \"Detailed error information\",\n              \"properties\": {\n                \"message\": {\n                  \"type\": \"string\",\n                  \"description\": \"Error message\",\n                  \"example\": \"This is an example description.\"\n                },\n                \"code\": {\n                  \"type\": \"string\",\n                  \"description\": \"Error code\",\n  \
  \                \"example\": \"example-value\"\n                },\n                \"in\": {\n                  \"type\": \"string\",\n                  \"description\": \"Field where error occurred\",\n                  \"example\": \"example-value\"\n                },\n                \"subCategory\": {\n                  \"type\": \"string\",\n                  \"description\": \"Error subcategory\",\n                  \"example\": \"standard\"\n                },\n                \"context\": {\n                  \"type\": \"object\",\n                  \"example\": {\n                    \"key\": \"value\"\n                  }\n                }\n              },\n              \"required\": [\n                \"message\"\n              ]\n            }\n          }\n        }\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"results\",\n    \"startedAt\"\
  ,\n    \"completedAt\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchNotesResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-notes-batch-notes-response-schema.json
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
title: BatchNotesResponse
---
