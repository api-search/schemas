---
description: A paginated list of HubDB tables.
layout: schema
name: CollectionResponseHubDBTable
properties_list:
- description: ''
  name: results
  type: array
- description: Pagination information.
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/cms-hubdb-api-collection-response-hub-dbtable-schema.json
slug: cms-hubdb-api-collection-response-hub-dbtable
source_filename: cms-hubdb-api-collection-response-hub-dbtable-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-hubdb-api-collection-response-hub-dbtable-schema.json\",\n  \"title\": \"CollectionResponseHubDBTable\",\n  \"description\": \"A paginated list of HubDB tables.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A HubDB table.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the table.\",\n            \"example\": \"500123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The machine-readable name of the table.\",\n            \"example\": \"Example Record\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n   \
  \         \"description\": \"The human-readable label for the table.\",\n            \"example\": \"Example Record\"\n          },\n          \"columns\": {\n            \"type\": \"array\",\n            \"description\": \"The column definitions for the table.\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/HubDBColumn\"\n            },\n            \"example\": [\n              {\n                \"id\": \"500123\",\n                \"name\": \"Example Record\",\n                \"label\": \"Example Record\",\n                \"type\": \"TEXT\",\n                \"options\": [\n                  {}\n                ]\n              }\n            ]\n          },\n          \"published\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the table has been published.\",\n            \"example\": true\n          },\n          \"rowCount\": {\n            \"type\": \"integer\",\n            \"description\": \"The number of rows in\
  \ the published table.\",\n            \"example\": 10\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The date and time the table was created.\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"updatedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The date and time the table was last updated.\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"publishedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The date and time the table was last published.\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"name\": \"Example Record\",\n          \"label\": \"Example Record\",\n          \"columns\"\
  : [\n            {\n              \"id\": \"500123\",\n              \"name\": \"Example Record\",\n              \"label\": \"Example Record\",\n              \"type\": \"TEXT\",\n              \"options\": [\n                {}\n              ]\n            }\n          ],\n          \"published\": true,\n          \"rowCount\": 10,\n          \"createdAt\": \"2025-03-15T14:30:00Z\",\n          \"updatedAt\": \"2025-03-15T14:30:00Z\",\n          \"publishedAt\": \"2025-03-15T14:30:00Z\"\n        }\n      ]\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information.\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\"\n            }\n          },\n          \"example\": {\n            \"after\": \"example-value\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-hubdb-api-collection-response-hub-dbtable-schema.json
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
title: CollectionResponseHubDBTable
---
