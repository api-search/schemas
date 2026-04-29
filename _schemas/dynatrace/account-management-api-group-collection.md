---
description: A paginated collection of groups.
layout: schema
name: GroupCollection
properties_list:
- description: Cursor for the next page of results.
  name: nextPageKey
  type: string
- description: The total number of groups in the account.
  name: totalCount
  type: integer
- description: The list of groups on this page.
  name: items
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/account-management-api-group-collection-schema.json
slug: account-management-api-group-collection
source_filename: account-management-api-group-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/account-management-api-group-collection-schema.json\",\n  \"title\": \"GroupCollection\",\n  \"description\": \"A paginated collection of groups.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page of results.\",\n      \"nullable\": true,\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The total number of groups in the account.\",\n      \"example\": 500\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"The list of groups on this page.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Group\"\n      },\n      \"example\": [\n        {\n          \"groupId\":\
  \ \"abc123\",\n          \"name\": \"Production Service\",\n          \"description\": \"Example description.\",\n          \"owner\": \"example-value\",\n          \"createdAt\": \"2025-03-15T14:30:00Z\",\n          \"updatedAt\": \"2025-03-15T14:30:00Z\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/account-management-api-group-collection-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: GroupCollection
---
