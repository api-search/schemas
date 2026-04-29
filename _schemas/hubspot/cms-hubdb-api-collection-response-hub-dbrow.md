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
schema_file: json-schema/cms-hubdb-api-collection-response-hub-dbrow-schema.json
slug: cms-hubdb-api-collection-response-hub-dbrow
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-hubdb-api-collection-response-hub-dbrow-schema.json\",\n  \"title\": \"CollectionResponseHubDBRow\",\n  \"description\": \"A paginated list of HubDB table rows.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A row in a HubDB table.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the row.\",\n            \"example\": \"500123\"\n          },\n          \"values\": {\n            \"type\": \"object\",\n            \"description\": \"The column values for the row as key-value pairs.\",\n            \"additionalProperties\": true,\n            \"example\": {\n              \"key\": \"value\"\
  \n            }\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The date and time the row was created.\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"updatedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The date and time the row was last updated.\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"values\": {\n            \"key\": \"value\"\n          },\n          \"createdAt\": \"2025-03-15T14:30:00Z\",\n          \"updatedAt\": \"2025-03-15T14:30:00Z\"\n        }\n      ]\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information.\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"properties\"\
  : {\n            \"after\": {\n              \"type\": \"string\"\n            }\n          },\n          \"example\": {\n            \"after\": \"example-value\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-hubdb-api-collection-response-hub-dbrow-schema.json
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
