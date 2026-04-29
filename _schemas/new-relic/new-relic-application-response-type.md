---
description: ''
layout: schema
name: ApplicationResponseType
properties_list:
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
  type: string
- description: ''
  name: last_reported_at
  type: string
- description: ''
  name: links
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: reporting
  type: boolean
- description: ''
  name: settings
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-application-response-type-schema.json
slug: new-relic-application-response-type
source_filename: new-relic-application-response-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"application_summary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"apdex_score\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 87.5\n        },\n        \"apdex_target\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 42.5\n        },\n        \"concurrent_instance_count\": {\n          \"type\": \"integer\",\n          \"example\": 42\n        },\n        \"error_rate\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 12.3\n        },\n        \"host_count\": {\n          \"type\": \"integer\",\n          \"example\": 42\n        },\n        \"instance_count\": {\n          \"type\": \"integer\",\n          \"example\": 42\n        },\n        \"response_time\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 42.5\n\
  \        },\n        \"throughput\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 42.5\n        }\n      }\n    },\n    \"end_user_summary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"apdex_score\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 87.5\n        },\n        \"apdex_target\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 42.5\n        },\n        \"response_time\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 42.5\n        },\n        \"throughput\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 42.5\n        }\n      }\n    },\n    \"health_status\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"language\": {\n\
  \      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"last_reported_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T14:30:00Z\"\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"servers\": {\n          \"type\": \"array\",\n          \"example\": [\n            100\n          ],\n          \"items\": {\n            \"type\": \"integer\"\n          }\n        },\n        \"application_hosts\": {\n          \"type\": \"array\",\n          \"example\": [\n            100\n          ],\n          \"items\": {\n            \"type\": \"integer\"\n          }\n        },\n        \"application_instances\": {\n          \"type\": \"array\",\n          \"example\": [\n            100\n          ],\n          \"items\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\
  \n    },\n    \"reporting\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"app_apdex_threshold\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 42.5\n        },\n        \"enable_real_user_monitoring\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"end_user_apdex_threshold\": {\n          \"type\": \"number\",\n          \"format\": \"float\",\n          \"example\": 42.5\n        },\n        \"use_server_side_config\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationResponseType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-application-response-type-schema.json
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
title: ApplicationResponseType
---
