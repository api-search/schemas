---
description: Response from batch operations
layout: schema
name: BatchResponse
properties_list:
- description: Current status of the batch operation
  name: status
  type: string
- description: Successfully processed authors
  name: results
  type: array
- description: ISO 8601 timestamp when the batch was requested
  name: requestedAt
  type: string
- description: ISO 8601 timestamp when processing started
  name: startedAt
  type: string
- description: ISO 8601 timestamp when processing completed
  name: completedAt
  type: string
- description: Related links for the batch operation
  name: links
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/authors-api-batch-response-schema.json
slug: authors-api-batch-response
source_filename: authors-api-batch-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-batch-response-schema.json\",\n  \"title\": \"BatchResponse\",\n  \"description\": \"Response from batch operations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING\",\n        \"PROCESSING\",\n        \"CANCELED\",\n        \"COMPLETE\"\n      ],\n      \"description\": \"Current status of the batch operation\",\n      \"example\": \"PENDING\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents a blog author profile with biographical and social information\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the blog author\",\n      \
  \      \"example\": \"500123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Full display name of the author\",\n            \"example\": \"Example Record\"\n          },\n          \"slug\": {\n            \"type\": \"string\",\n            \"description\": \"URL-friendly identifier for the author\",\n            \"example\": \"example-value\"\n          },\n          \"email\": {\n            \"type\": \"string\",\n            \"format\": \"email\",\n            \"description\": \"Author's email address\",\n            \"example\": \"jsmith@example.com\"\n          },\n          \"bio\": {\n            \"type\": \"string\",\n            \"description\": \"Author biography or description\",\n            \"example\": \"example-value\"\n          },\n          \"website\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"Author's personal website URL\",\n            \"example\"\
  : \"https://app.hubspot.com/contacts/12345\"\n          },\n          \"twitter\": {\n            \"type\": \"string\",\n            \"description\": \"Author's Twitter/X handle\",\n            \"example\": \"example-value\"\n          },\n          \"facebook\": {\n            \"type\": \"string\",\n            \"description\": \"Author's Facebook profile URL\",\n            \"example\": \"example-value\"\n          },\n          \"linkedin\": {\n            \"type\": \"string\",\n            \"description\": \"Author's LinkedIn profile URL\",\n            \"example\": \"https://app.hubspot.com/contacts/12345\"\n          },\n          \"avatar\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"URL to the author's avatar image\",\n            \"example\": \"https://app.hubspot.com/contacts/12345\"\n          },\n          \"language\": {\n            \"type\": \"string\",\n            \"description\": \"Language code for the author\
  \ profile (e.g., en, es, fr)\",\n            \"example\": \"en\"\n          },\n          \"translatedFromId\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the original author this was translated from\",\n            \"example\": \"500123\"\n          },\n          \"created\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"ISO 8601 timestamp when the author was created\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"updated\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"ISO 8601 timestamp when the author was last updated\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"deletedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"ISO 8601 timestamp when the author was archived\",\n            \"example\": \"\
  2025-03-15T14:30:00Z\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"name\",\n          \"created\",\n          \"updated\"\n        ]\n      },\n      \"description\": \"Successfully processed authors\",\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"name\": \"Example Record\",\n          \"slug\": \"example-value\",\n          \"email\": \"jsmith@example.com\",\n          \"bio\": \"example-value\",\n          \"website\": \"https://app.hubspot.com/contacts/12345\",\n          \"twitter\": \"example-value\",\n          \"facebook\": \"example-value\",\n          \"linkedin\": \"https://app.hubspot.com/contacts/12345\",\n          \"avatar\": \"https://app.hubspot.com/contacts/12345\",\n          \"language\": \"en\",\n          \"translatedFromId\": \"500123\",\n          \"created\": \"2025-03-15T14:30:00Z\",\n          \"updated\": \"2025-03-15T14:30:00Z\",\n          \"deletedAt\": \"2025-03-15T14:30:00Z\"\n       \
  \ }\n      ]\n    },\n    \"requestedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the batch was requested\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when processing started\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when processing completed\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Related links for the batch operation\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"results\",\n    \"startedAt\",\n \
  \   \"completedAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-batch-response-schema.json
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
title: BatchResponse
---
