---
description: ''
layout: schema
name: ViolationResponseType
properties_list:
- description: ''
  name: closed_at
  type: integer
- description: ''
  name: condition_name
  type: string
- description: ''
  name: duration
  type: integer
- description: ''
  name: entity
  type: object
- description: ''
  name: id
  type: integer
- description: ''
  name: label
  type: string
- description: ''
  name: links
  type: object
- description: ''
  name: opened_at
  type: integer
- description: ''
  name: policy_name
  type: string
- description: ''
  name: priority
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-violation-response-type-schema.json
slug: new-relic-violation-response-type
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"closed_at\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"condition_name\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"entity\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"group_id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"example-resource-01\"\n        },\n        \"product\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"standard\"\n        }\n      }\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\"\
  : 100\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"condition_id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"incident_id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"policy_id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        }\n      }\n    },\n    \"opened_at\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"policy_name\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ViolationResponseType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-violation-response-type-schema.json
tags:
- Analysis
- Analytics
- APM
- DevOps
- Infrastructure
- Monitoring
- Observability
- Performance
- Platform
title: ViolationResponseType
---
