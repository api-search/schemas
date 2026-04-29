---
description: Response from a batch read operation
layout: schema
name: BatchReadResponse
properties_list:
- description: The status of the batch operation
  name: status
  type: string
- description: The retrieved commerce payments
  name: results
  type: array
- description: When the request was received
  name: requestedAt
  type: string
- description: When processing started
  name: startedAt
  type: string
- description: When processing completed
  name: completedAt
  type: string
- description: Number of errors encountered
  name: numErrors
  type: integer
- description: List of errors
  name: errors
  type: array
- description: ''
  name: links
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/commerce-payments-api-batch-read-response-schema.json
slug: commerce-payments-api-batch-read-response
source_filename: commerce-payments-api-batch-read-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-batch-read-response-schema.json\",\n  \"title\": \"BatchReadResponse\",\n  \"description\": \"Response from a batch read operation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING\",\n        \"PROCESSING\",\n        \"CANCELED\",\n        \"COMPLETE\"\n      ],\n      \"description\": \"The status of the batch operation\",\n      \"example\": \"PENDING\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"The retrieved commerce payments\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A commerce payment object representing a payment transaction\",\n        \"required\": [\n          \"id\",\n          \"properties\",\n          \"createdAt\"\
  ,\n          \"updatedAt\"\n        ],\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the commerce payment\",\n            \"example\": \"500123\"\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The properties of the commerce payment\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"When the commerce payment was created\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"updatedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"When the commerce payment was last updated\",\n\
  \            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"archived\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the commerce payment is archived\",\n            \"example\": true\n          },\n          \"archivedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"When the commerce payment was archived\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"associations\": {\n            \"type\": \"object\",\n            \"description\": \"Associated objects\",\n            \"additionalProperties\": {\n              \"$ref\": \"#/components/schemas/AssociationResult\"\n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"propertiesWithHistory\": {\n            \"type\": \"object\",\n            \"description\": \"Properties with their value history\",\n            \"additionalProperties\"\
  : {\n              \"type\": \"array\",\n              \"items\": {\n                \"$ref\": \"#/components/schemas/PropertyHistory\"\n              }\n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"properties\": {\n            \"key\": \"value\"\n          },\n          \"createdAt\": \"2025-03-15T14:30:00Z\",\n          \"updatedAt\": \"2025-03-15T14:30:00Z\",\n          \"archived\": true,\n          \"archivedAt\": \"2025-03-15T14:30:00Z\",\n          \"associations\": {\n            \"key\": \"value\"\n          },\n          \"propertiesWithHistory\": {\n            \"key\": \"value\"\n          }\n        }\n      ]\n    },\n    \"requestedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the request was received\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n  \
  \  \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When processing started\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When processing completed\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"numErrors\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of errors encountered\",\n      \"example\": 100\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of errors\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"An error from a batch operation\",\n        \"required\": [\n          \"category\",\n          \"message\"\n        ],\n        \"properties\": {\n          \"status\": {\n            \"type\": \"string\",\n            \"example\": \"active\"\n          },\n          \"id\": {\n            \"type\": \"\
  string\",\n            \"example\": \"500123\"\n          },\n          \"category\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"example\": \"This is an example description.\"\n          },\n          \"errors\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/ErrorDetail\"\n            },\n            \"example\": [\n              {\n                \"message\": \"This is an example description.\",\n                \"code\": \"example-value\",\n                \"in\": \"example-value\",\n                \"subCategory\": \"standard\",\n                \"context\": {\n                  \"key\": \"value\"\n                }\n              }\n            ]\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"array\",\n\
  \              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"links\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"subCategory\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"status\": \"active\",\n          \"id\": \"500123\",\n          \"category\": \"standard\",\n          \"message\": \"This is an example description.\",\n          \"errors\": [\n            {}\n          ],\n          \"context\": {\n            \"key\": \"value\"\n          },\n          \"links\": {\n            \"key\": \"value\"\n          },\n          \"subCategory\": \"standard\"\
  \n        }\n      ]\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"results\",\n    \"startedAt\",\n    \"completedAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-batch-read-response-schema.json
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
title: BatchReadResponse
---
