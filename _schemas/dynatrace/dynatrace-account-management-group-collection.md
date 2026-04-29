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
schema_file: json-schema/dynatrace-account-management-group-collection-schema.json
slug: dynatrace-account-management-group-collection
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A paginated collection of groups.\",\n  \"properties\": {\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page of results.\",\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of groups in the account.\",\n      \"format\": \"int64\",\n      \"example\": 500\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"The list of groups on this page.\",\n      \"example\": [\n        {\n          \"groupId\": \"abc123\",\n          \"name\": \"Production Service\",\n          \"description\": \"Example description.\",\n          \"owner\": \"example-value\",\n          \"createdAt\": \"2025-03-15T14:30:00Z\",\n          \"updatedAt\": \"2025-03-15T14:30:00Z\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents\
  \ a user group in the Dynatrace account.\",\n        \"properties\": {\n          \"groupId\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the group.\",\n            \"example\": \"abc123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The display name of the group.\",\n            \"example\": \"Production Service\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"An optional description of the group's purpose or scope.\",\n            \"example\": \"Example description.\"\n          },\n          \"owner\": {\n            \"type\": \"string\",\n            \"description\": \"The identifier of the group owner. LOCAL indicates the group is managed within Dynatrace; SSO indicates it is synced from an identity provider.\",\n            \"example\": \"example-value\"\n          },\n          \"createdAt\": {\n           \
  \ \"type\": \"string\",\n            \"description\": \"The date and time when the group was created.\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"updatedAt\": {\n            \"type\": \"string\",\n            \"description\": \"The date and time when the group was last updated.\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-account-management-group-collection-schema.json
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
