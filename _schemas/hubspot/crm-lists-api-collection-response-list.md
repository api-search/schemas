---
description: A paginated list of CRM lists.
layout: schema
name: CollectionResponseList
properties_list:
- description: ''
  name: results
  type: array
- description: Pagination information.
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-lists-api-collection-response-list-schema.json
slug: crm-lists-api-collection-response-list
source_filename: crm-lists-api-collection-response-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-lists-api-collection-response-list-schema.json\",\n  \"title\": \"CollectionResponseList\",\n  \"description\": \"A paginated list of CRM lists.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A HubSpot CRM list.\",\n        \"properties\": {\n          \"listId\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the list.\",\n            \"example\": \"500123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the list.\",\n            \"example\": \"Example Record\"\n          },\n          \"listType\": {\n            \"type\": \"string\",\n            \"enum\": [\n \
  \             \"STATIC\",\n              \"DYNAMIC\"\n            ],\n            \"description\": \"Whether the list is static (manually managed) or dynamic (filter-based).\",\n            \"example\": \"STATIC\"\n          },\n          \"objectTypeId\": {\n            \"type\": \"string\",\n            \"description\": \"The object type the list contains (e.g., 0-1 for contacts).\",\n            \"example\": \"500123\"\n          },\n          \"processingStatus\": {\n            \"type\": \"string\",\n            \"description\": \"The current processing status of the list.\",\n            \"example\": \"active\"\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The date and time the list was created.\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"updatedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"\
  description\": \"The date and time the list was last updated.\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"filterBranch\": {\n            \"type\": \"object\",\n            \"description\": \"The filter definition for dynamic lists.\",\n            \"example\": {}\n          },\n          \"memberCount\": {\n            \"type\": \"integer\",\n            \"description\": \"The current number of members in the list.\",\n            \"example\": 10\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"listId\": \"500123\",\n          \"name\": \"Example Record\",\n          \"listType\": \"STATIC\",\n          \"objectTypeId\": \"500123\",\n          \"processingStatus\": \"active\",\n          \"createdAt\": \"2025-03-15T14:30:00Z\",\n          \"updatedAt\": \"2025-03-15T14:30:00Z\",\n          \"filterBranch\": {},\n          \"memberCount\": 10\n        }\n      ]\n    },\n    \"paging\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"Pagination information.\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\"\n            }\n          },\n          \"example\": {\n            \"after\": \"example-value\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-lists-api-collection-response-list-schema.json
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
title: CollectionResponseList
---
