---
description: Request body for creating or updating a user.
layout: schema
name: UserCreateRequest
properties_list:
- description: The email address of the user. Used as the login identifier.
  name: email
  type: string
- description: The first name of the user.
  name: firstName
  type: string
- description: The last name of the user.
  name: lastName
  type: string
- description: The list of group IDs to assign the user to. The user gains all permissions associated with these groups.
  name: groups
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-account-management-user-create-request-schema.json
slug: dynatrace-account-management-user-create-request
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for creating or updating a user.\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the user. Used as the login identifier.\",\n      \"format\": \"email\",\n      \"example\": \"admin@example.com\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"The first name of the user.\",\n      \"example\": \"Production Service\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"The last name of the user.\",\n      \"example\": \"Production Service\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"The list of group IDs to assign the user to. The user gains all permissions associated with these groups.\",\n      \"example\": [\n        \"example-value\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n  \
  \  \"email\",\n    \"firstName\",\n    \"lastName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserCreateRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-account-management-user-create-request-schema.json
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
title: UserCreateRequest
---
