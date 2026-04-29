---
description: ''
layout: schema
name: ApplicationHostResponseType
properties_list:
- description: ''
  name: host
  type: string
- description: ''
  name: application_name
  type: string
- description: ''
  name: application_summary
  type: object
- description: ''
  name: end_user_summary
  type: object
- description: ''
  name: health_status
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: language
  type: integer
- description: ''
  name: links
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-application-host-response-type-schema.json
slug: new-relic-application-host-response-type
source_filename: new-relic-application-host-response-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"host\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"application_name\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"application_summary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"apdex_score\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 87.5\n        },\n        \"error_rate\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 12.3\n        },\n        \"instance_count\": {\n          \"type\": \"integer\",\n          \"example\": 42\n        },\n        \"response_time\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 42.5\n        },\n        \"throughput\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 42.5\n        }\n      }\n\
  \    },\n    \"end_user_summary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"apdex_score\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 87.5\n        },\n        \"response_time\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 42.5\n        },\n        \"throughput\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 42.5\n        }\n      }\n    },\n    \"health_status\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"language\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"application\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"application_instances\": {\n          \"type\"\
  : \"array\",\n          \"example\": [\n            100\n          ],\n          \"items\": {\n            \"type\": \"integer\"\n          }\n        },\n        \"server\": {\n          \"type\": \"integer\",\n          \"example\": 100\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationHostResponseType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-application-host-response-type-schema.json
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
title: ApplicationHostResponseType
---
