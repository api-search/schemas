---
description: ''
layout: schema
name: ApplicationHostResponse
properties_list:
- description: ''
  name: application_hosts
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-application-host-response-schema.json
slug: new-relic-application-host-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"application_hosts\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"host\": \"example_string\",\n          \"application_name\": \"example_string\",\n          \"application_summary\": {},\n          \"end_user_summary\": {},\n          \"health_status\": \"active\",\n          \"id\": 100,\n          \"language\": 100,\n          \"links\": {}\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"host\": {\n            \"type\": \"string\",\n            \"example\": \"example_string\"\n          },\n          \"application_name\": {\n            \"type\": \"string\",\n            \"example\": \"example_string\"\n          },\n          \"application_summary\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"apdex_score\": {\n                \"type\": \"number\",\n                \"format\": \"float\"\
  ,\n                \"example\": 87.5\n              },\n              \"error_rate\": {\n                \"type\": \"number\",\n                \"format\": \"float\",\n                \"example\": 12.3\n              },\n              \"instance_count\": {\n                \"type\": \"integer\",\n                \"example\": 42\n              },\n              \"response_time\": {\n                \"type\": \"number\",\n                \"format\": \"float\",\n                \"example\": 42.5\n              },\n              \"throughput\": {\n                \"type\": \"number\",\n                \"format\": \"float\",\n                \"example\": 42.5\n              }\n            }\n          },\n          \"end_user_summary\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"apdex_score\": {\n                \"type\": \"number\",\n                \"format\": \"float\",\n                \"example\": 87.5\n              },\n              \"response_time\"\
  : {\n                \"type\": \"number\",\n                \"format\": \"float\",\n                \"example\": 42.5\n              },\n              \"throughput\": {\n                \"type\": \"number\",\n                \"format\": \"float\",\n                \"example\": 42.5\n              }\n            }\n          },\n          \"health_status\": {\n            \"type\": \"string\",\n            \"example\": \"active\"\n          },\n          \"id\": {\n            \"type\": \"integer\",\n            \"example\": 100\n          },\n          \"language\": {\n            \"type\": \"integer\",\n            \"example\": 100\n          },\n          \"links\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"application\": {\n                \"type\": \"integer\",\n                \"example\": 100\n              },\n              \"application_instances\": {\n                \"type\": \"array\",\n                \"example\": [\n             \
  \     100\n                ],\n                \"items\": {\n                  \"type\": \"integer\"\n                }\n              },\n              \"server\": {\n                \"type\": \"integer\",\n                \"example\": 100\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationHostResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-application-host-response-schema.json
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
title: ApplicationHostResponse
---
