---
description: Response from batch association operations
layout: schema
name: BatchAssociationResponse
properties_list:
- description: Status of the batch operation
  name: status
  type: string
- description: Successfully processed associations
  name: results
  type: array
- description: When the batch was requested
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
schema_file: json-schema/crm-associations-api-batch-association-response-schema.json
slug: crm-associations-api-batch-association-response
source_filename: crm-associations-api-batch-association-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-batch-association-response-schema.json\",\n  \"title\": \"BatchAssociationResponse\",\n  \"description\": \"Response from batch association operations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING\",\n        \"PROCESSING\",\n        \"CANCELED\",\n        \"COMPLETE\"\n      ],\n      \"description\": \"Status of the batch operation\",\n      \"example\": \"PENDING\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Result of an association query\",\n        \"properties\": {\n          \"from\": {\n            \"$ref\": \"#/components/schemas/ObjectReference\"\n          },\n          \"to\": {\n            \"type\"\
  : \"array\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/Association\"\n            },\n            \"description\": \"Associated objects\",\n            \"example\": [\n              {\n                \"toObjectId\": \"500123\",\n                \"associationTypes\": [\n                  {\n                    \"associationCategory\": \"HUBSPOT_DEFINED\",\n                    \"associationTypeId\": 500123,\n                    \"label\": \"Example Record\"\n                  }\n                ]\n              }\n            ]\n          },\n          \"paging\": {\n            \"$ref\": \"#/components/schemas/Paging\"\n          }\n        },\n        \"required\": [\n          \"from\",\n          \"to\"\n        ]\n      },\n      \"description\": \"Successfully processed associations\",\n      \"example\": [\n        {\n          \"from\": {},\n          \"to\": [\n            {\n              \"toObjectId\": \"500123\",\n              \"associationTypes\"\
  : [\n                {\n                  \"associationCategory\": \"HUBSPOT_DEFINED\",\n                  \"associationTypeId\": 500123,\n                  \"label\": \"Example Record\"\n                }\n              ]\n            }\n          ],\n          \"paging\": {}\n        }\n      ]\n    },\n    \"requestedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the batch was requested\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When processing started\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When processing completed\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"numErrors\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of errors encountered\",\n\
  \      \"example\": 100\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Standard error in batch operations\",\n        \"properties\": {\n          \"status\": {\n            \"type\": \"string\",\n            \"example\": \"active\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"category\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"example\": \"This is an example description.\"\n          },\n          \"errors\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/ErrorDetail\"\n            },\n            \"example\": [\n              {\n                \"message\": \"This is an example description.\",\n                \"code\": \"example-value\"\
  ,\n                \"subCategory\": \"standard\",\n                \"in\": \"example-value\",\n                \"context\": {\n                  \"key\": \"value\"\n                }\n              }\n            ]\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"links\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        },\n        \"required\": [\n          \"status\",\n          \"category\",\n          \"message\"\n        ]\n      },\n      \"description\": \"List of errors\",\n      \"example\": [\n    \
  \    {\n          \"status\": \"active\",\n          \"id\": \"500123\",\n          \"category\": \"standard\",\n          \"message\": \"This is an example description.\",\n          \"errors\": [\n            {}\n          ],\n          \"context\": {\n            \"key\": \"value\"\n          },\n          \"links\": {\n            \"key\": \"value\"\n          }\n        }\n      ]\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"results\",\n    \"startedAt\",\n    \"completedAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-batch-association-response-schema.json
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
title: BatchAssociationResponse
---
