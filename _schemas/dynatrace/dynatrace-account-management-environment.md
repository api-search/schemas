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
schema_file: json-schema/dynatrace-account-management-environment-schema.json
slug: dynatrace-account-management-environment
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Represents a Dynatrace environment (tenant) associated with the account.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique environment identifier (tenant ID).\",\n      \"example\": \"abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the environment.\",\n      \"example\": \"Production Service\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the environment.\",\n      \"example\": \"ACTIVE\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"SUSPENDED\",\n        \"TRIAL\"\n      ]\n    },\n    \"trial\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the environment is a trial environment.\",\n      \"example\": true\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Environment\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-account-management-environment-schema.json
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
