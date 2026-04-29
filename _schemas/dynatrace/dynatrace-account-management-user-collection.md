---
description: A paginated collection of users.
layout: schema
name: UserCollection
properties_list:
- description: Cursor for the next page of results.
  name: nextPageKey
  type: string
- description: The total number of users in the account.
  name: totalCount
  type: integer
- description: The list of users on this page.
  name: items
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-account-management-user-collection-schema.json
slug: dynatrace-account-management-user-collection
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A paginated collection of users.\",\n  \"properties\": {\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page of results.\",\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of users in the account.\",\n      \"format\": \"int64\",\n      \"example\": 500\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"The list of users on this page.\",\n      \"example\": [\n        {\n          \"uid\": \"abc123\",\n          \"email\": \"admin@example.com\",\n          \"firstName\": \"Production Service\",\n          \"lastName\": \"Production Service\",\n          \"groups\": [\n            \"example-value\"\n          ],\n          \"userStatus\": \"ACTIVE\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents\
  \ a user in the Dynatrace account.\",\n        \"properties\": {\n          \"uid\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the user.\",\n            \"example\": \"abc123\"\n          },\n          \"email\": {\n            \"type\": \"string\",\n            \"description\": \"The email address of the user, used as their login identifier.\",\n            \"format\": \"email\",\n            \"example\": \"admin@example.com\"\n          },\n          \"firstName\": {\n            \"type\": \"string\",\n            \"description\": \"The first name of the user.\",\n            \"example\": \"Production Service\"\n          },\n          \"lastName\": {\n            \"type\": \"string\",\n            \"description\": \"The last name of the user.\",\n            \"example\": \"Production Service\"\n          },\n          \"groups\": {\n            \"type\": \"array\",\n            \"description\": \"The list of group IDs that the user\
  \ belongs to.\",\n            \"example\": [\n              \"example-value\"\n            ],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"userStatus\": {\n            \"type\": \"string\",\n            \"description\": \"The current status of the user account.\",\n            \"example\": \"ACTIVE\",\n            \"enum\": [\n              \"ACTIVE\",\n              \"INACTIVE\",\n              \"PENDING_INVITE\"\n            ]\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-account-management-user-collection-schema.json
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
title: UserCollection
---
