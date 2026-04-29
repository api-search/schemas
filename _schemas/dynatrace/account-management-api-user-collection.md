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
schema_file: json-schema/account-management-api-user-collection-schema.json
slug: account-management-api-user-collection
source_filename: account-management-api-user-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/account-management-api-user-collection-schema.json\",\n  \"title\": \"UserCollection\",\n  \"description\": \"A paginated collection of users.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page of results.\",\n      \"nullable\": true,\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The total number of users in the account.\",\n      \"example\": 500\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"The list of users on this page.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/User\"\n      },\n      \"example\": [\n        {\n          \"uid\": \"abc123\"\
  ,\n          \"email\": \"admin@example.com\",\n          \"firstName\": \"Production Service\",\n          \"lastName\": \"Production Service\",\n          \"groups\": [\n            \"example-value\"\n          ],\n          \"userStatus\": \"ACTIVE\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/account-management-api-user-collection-schema.json
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
