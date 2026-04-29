---
description: ''
layout: schema
name: MobileApplicationResponse
properties_list:
- description: ''
  name: application
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-mobile-application-response-schema.json
slug: new-relic-mobile-application-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"crash_summary\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"crash_count\": {\n              \"type\": \"integer\",\n              \"example\": 42\n            },\n            \"crash_rate\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 12.3\n            },\n            \"supports_crash_data\": {\n              \"type\": \"boolean\",\n              \"example\": true\n            },\n            \"unresolved_crash_count\": {\n              \"type\": \"integer\",\n              \"example\": 42\n            }\n          }\n        },\n        \"health_status\": {\n          \"type\": \"string\",\n          \"example\": \"active\"\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"mobile_summary\"\
  : {\n          \"type\": \"object\",\n          \"properties\": {\n            \"active_users\": {\n              \"type\": \"integer\",\n              \"example\": 100\n            },\n            \"calls_per_session\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 42.5\n            },\n            \"failed_call_rate\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 12.3\n            },\n            \"interaction_time\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 42.5\n            },\n            \"launch_count\": {\n              \"type\": \"integer\",\n              \"example\": 42\n            },\n            \"remote_error_rate\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 12.3\n            },\n            \"response_time\": {\n              \"\
  type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 42.5\n            },\n            \"throughput\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"example\": 42.5\n            }\n          }\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"example-resource-01\"\n        },\n        \"reporting\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MobileApplicationResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-mobile-application-response-schema.json
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
title: MobileApplicationResponse
---
