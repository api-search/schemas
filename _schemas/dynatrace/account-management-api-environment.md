---
description: Represents a Dynatrace environment (tenant) associated with the account.
layout: schema
name: Environment
properties_list:
- description: The unique environment identifier (tenant ID).
  name: id
  type: string
- description: The display name of the environment.
  name: name
  type: string
- description: The current status of the environment.
  name: status
  type: string
- description: Whether the environment is a trial environment.
  name: trial
  type: boolean
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/account-management-api-environment-schema.json
slug: account-management-api-environment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/account-management-api-environment-schema.json\",\n  \"title\": \"Environment\",\n  \"description\": \"Represents a Dynatrace environment (tenant) associated with the account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique environment identifier (tenant ID).\",\n      \"example\": \"abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the environment.\",\n      \"example\": \"Production Service\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the environment.\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"SUSPENDED\",\n        \"TRIAL\"\n      ],\n      \"example\": \"ACTIVE\"\n    },\n    \"trial\": {\n    \
  \  \"type\": \"boolean\",\n      \"description\": \"Whether the environment is a trial environment.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/account-management-api-environment-schema.json
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
title: Environment
---
