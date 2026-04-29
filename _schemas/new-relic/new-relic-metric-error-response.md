---
description: Error response body
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: error
  type: object
- description: List of individual failure details when partial rejection occurs
  name: failures
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-metric-error-response-schema.json
slug: new-relic-metric-error-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Error response body\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"type\": \"standard\",\n        \"message\": \"Operation completed successfully\"\n      },\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Error type identifier\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable error description\"\n        }\n      }\n    },\n    \"failures\": {\n      \"type\": \"array\",\n      \"description\": \"List of individual failure details when partial rejection occurs\",\n      \"example\": [\n        {\n          \"error\": {\n            \"message\": \"Operation completed successfully\"\n          },\n          \"failed\": [\n            {}\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n\
  \          \"error\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"message\": {\n                \"type\": \"string\"\n              }\n            }\n          },\n          \"failed\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-metric-error-response-schema.json
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
title: ErrorResponse
---
