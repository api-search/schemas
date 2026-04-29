---
description: A paginated collection of environments.
layout: schema
name: EnvironmentCollection
properties_list:
- description: Cursor for the next page of results.
  name: nextPageKey
  type: string
- description: The total number of environments in the account.
  name: totalCount
  type: integer
- description: The list of environments on this page.
  name: environments
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-account-management-environment-collection-schema.json
slug: dynatrace-account-management-environment-collection
source_filename: dynatrace-account-management-environment-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A paginated collection of environments.\",\n  \"properties\": {\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page of results.\",\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of environments in the account.\",\n      \"format\": \"int64\",\n      \"example\": 500\n    },\n    \"environments\": {\n      \"type\": \"array\",\n      \"description\": \"The list of environments on this page.\",\n      \"example\": [\n        {\n          \"id\": \"abc123\",\n          \"name\": \"Production Service\",\n          \"status\": \"ACTIVE\",\n          \"trial\": true\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents a Dynatrace environment (tenant) associated with the account.\",\n        \"properties\": {\n          \"id\": {\n\
  \            \"type\": \"string\",\n            \"description\": \"The unique environment identifier (tenant ID).\",\n            \"example\": \"abc123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The display name of the environment.\",\n            \"example\": \"Production Service\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"description\": \"The current status of the environment.\",\n            \"example\": \"ACTIVE\",\n            \"enum\": [\n              \"ACTIVE\",\n              \"SUSPENDED\",\n              \"TRIAL\"\n            ]\n          },\n          \"trial\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the environment is a trial environment.\",\n            \"example\": true\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvironmentCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-account-management-environment-collection-schema.json
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
title: EnvironmentCollection
---
