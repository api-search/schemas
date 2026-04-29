---
description: Represents a user in the Dynatrace account.
layout: schema
name: User
properties_list:
- description: The unique identifier of the user.
  name: uid
  type: string
- description: The email address of the user, used as their login identifier.
  name: email
  type: string
- description: The first name of the user.
  name: firstName
  type: string
- description: The last name of the user.
  name: lastName
  type: string
- description: The list of group IDs that the user belongs to.
  name: groups
  type: array
- description: The current status of the user account.
  name: userStatus
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/account-management-api-user-schema.json
slug: account-management-api-user
source_filename: account-management-api-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/account-management-api-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"Represents a user in the Dynatrace account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uid\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the user.\",\n      \"example\": \"abc123\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the user, used as their login identifier.\",\n      \"example\": \"admin@example.com\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"The first name of the user.\",\n      \"example\": \"Production Service\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"The last name of the user.\",\n   \
  \   \"example\": \"Production Service\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"The list of group IDs that the user belongs to.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"example-value\"\n      ]\n    },\n    \"userStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the user account.\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\",\n        \"PENDING_INVITE\"\n      ],\n      \"example\": \"ACTIVE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/account-management-api-user-schema.json
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
title: User
---
