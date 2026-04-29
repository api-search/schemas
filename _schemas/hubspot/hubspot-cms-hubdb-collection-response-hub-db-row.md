---
description: A paginated list of HubDB table rows.
layout: schema
name: CollectionResponseHubDBRow
properties_list:
- description: ''
  name: results
  type: array
- description: Pagination information.
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-cms-hubdb-collection-response-hub-db-row-schema.json
slug: hubspot-cms-hubdb-collection-response-hub-db-row
source_filename: hubspot-cms-hubdb-collection-response-hub-db-row-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A paginated list of HubDB table rows.\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"values\": {\n            \"key\": \"value\"\n          },\n          \"createdAt\": \"2025-03-15T14:30:00Z\",\n          \"updatedAt\": \"2025-03-15T14:30:00Z\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A row in a HubDB table.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the row.\",\n            \"example\": \"500123\"\n          },\n          \"values\": {\n            \"type\": \"object\",\n            \"description\": \"The column values for the row as key-value pairs.\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"createdAt\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"The date and time the row was created.\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"updatedAt\": {\n            \"type\": \"string\",\n            \"description\": \"The date and time the row was last updated.\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          }\n        }\n      }\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information.\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"example\": {\n            \"after\": \"example-value\"\n          },\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CollectionResponseHubDBRow\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-cms-hubdb-collection-response-hub-db-row-schema.json
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
title: CollectionResponseHubDBRow
---
