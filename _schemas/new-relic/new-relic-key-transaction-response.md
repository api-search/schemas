---
description: ''
layout: schema
name: KeyTransactionResponse
properties_list:
- description: ''
  name: key_transaction
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-key-transaction-response-schema.json
slug: new-relic-key-transaction-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"key_transaction\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"application_summary\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"apdex_score\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 87.5\n            },\n            \"apdex_target\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 42.5\n            },\n            \"concurrent_instance_count\": {\n              \"type\": \"integer\",\n              \"example\": 42\n            },\n            \"error_rate\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 12.3\n            },\n            \"host_count\": {\n              \"type\": \"integer\",\n              \"example\": 42\n            },\n            \"instance_count\": {\n        \
  \      \"type\": \"integer\",\n              \"example\": 42\n            },\n            \"response_time\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 42.5\n            },\n            \"throughput\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 42.5\n            }\n          }\n        },\n        \"end_user_summary\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"apdex_score\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 87.5\n            },\n            \"apdex_target\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 42.5\n            },\n            \"response_time\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 42.5\n            },\n            \"throughput\"\
  : {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 42.5\n            }\n          }\n        },\n        \"health_status\": {\n          \"type\": \"string\",\n          \"example\": \"active\"\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"last_reported_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"example\": \"2026-04-18T14:30:00Z\"\n        },\n        \"links\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"application\": {\n              \"type\": \"integer\",\n              \"description\": \"Application from which this key transaction originated\",\n              \"example\": 100\n            }\n          }\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"example-resource-01\"\n        },\n        \"reporting\": {\n          \"type\": \"\
  boolean\",\n          \"example\": true\n        },\n        \"transaction_name\": {\n          \"type\": \"string\",\n          \"example\": \"example_string\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyTransactionResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-key-transaction-response-schema.json
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
title: KeyTransactionResponse
---
