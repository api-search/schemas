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
schema_file: json-schema/account-management-api-environment-collection-schema.json
slug: account-management-api-environment-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/account-management-api-environment-collection-schema.json\",\n  \"title\": \"EnvironmentCollection\",\n  \"description\": \"A paginated collection of environments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page of results.\",\n      \"nullable\": true,\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The total number of environments in the account.\",\n      \"example\": 500\n    },\n    \"environments\": {\n      \"type\": \"array\",\n      \"description\": \"The list of environments on this page.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Environment\"\n      },\n      \"example\"\
  : [\n        {\n          \"id\": \"abc123\",\n          \"name\": \"Production Service\",\n          \"status\": \"ACTIVE\",\n          \"trial\": true\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/account-management-api-environment-collection-schema.json
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
