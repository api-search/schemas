---
description: ''
layout: schema
name: ViolationResponse
properties_list:
- description: ''
  name: violation
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-violation-response-schema.json
slug: new-relic-violation-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"violation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"closed_at\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"condition_name\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"duration\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"entity\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"group_id\": {\n              \"type\": \"integer\",\n              \"example\": 100\n            },\n            \"id\": {\n              \"type\": \"integer\",\n              \"example\": 100\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"example\": \"example-resource-01\"\n            },\n            \"product\": {\n              \"type\": \"string\",\n              \"example\": \"example_string\"\
  \n            },\n            \"type\": {\n              \"type\": \"string\",\n              \"example\": \"standard\"\n            }\n          }\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        },\n        \"links\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"condition_id\": {\n              \"type\": \"integer\",\n              \"example\": 100\n            },\n            \"incident_id\": {\n              \"type\": \"integer\",\n              \"example\": 100\n            },\n            \"policy_id\": {\n              \"type\": \"integer\",\n              \"example\": 100\n            }\n          }\n        },\n        \"opened_at\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"policy_name\": {\n          \"type\": \"string\",\n          \"example\"\
  : \"example_string\"\n        },\n        \"priority\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ViolationResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-violation-response-schema.json
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
title: ViolationResponse
---
