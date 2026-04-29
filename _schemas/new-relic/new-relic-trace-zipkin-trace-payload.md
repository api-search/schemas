---
description: Zipkin JSON v2 format trace payload
layout: schema
name: ZipkinTracePayload
properties_list: []
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-trace-zipkin-trace-payload-schema.json
slug: new-relic-trace-zipkin-trace-payload
source_filename: new-relic-trace-zipkin-trace-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"description\": \"Zipkin JSON v2 format trace payload\",\n  \"items\": {\n    \"type\": \"object\",\n    \"description\": \"A single span in Zipkin JSON v2 format\",\n    \"properties\": {\n      \"id\": {\n        \"type\": \"string\",\n        \"description\": \"Span ID (16 hex characters)\",\n        \"example\": \"500123\"\n      },\n      \"traceId\": {\n        \"type\": \"string\",\n        \"description\": \"Trace ID (32 hex characters)\",\n        \"example\": \"500123\"\n      },\n      \"parentId\": {\n        \"type\": \"string\",\n        \"description\": \"Parent span ID\",\n        \"example\": \"500123\"\n      },\n      \"name\": {\n        \"type\": \"string\",\n        \"description\": \"Span name / operation name\",\n        \"example\": \"example-resource-01\"\n      },\n      \"timestamp\": {\n        \"type\": \"integer\",\n        \"description\": \"Span start time in microseconds since epoch\",\n        \"example\": 1718153645993\n\
  \      },\n      \"duration\": {\n        \"type\": \"integer\",\n        \"description\": \"Span duration in microseconds\",\n        \"example\": 100\n      },\n      \"kind\": {\n        \"type\": \"string\",\n        \"example\": \"CLIENT\",\n        \"enum\": [\n          \"CLIENT\",\n          \"SERVER\",\n          \"PRODUCER\",\n          \"CONSUMER\"\n        ]\n      },\n      \"localEndpoint\": {\n        \"type\": \"object\",\n        \"example\": {\n          \"serviceName\": \"myService\",\n          \"ipv4\": \"example_string\",\n          \"port\": 8080\n        },\n        \"properties\": {\n          \"serviceName\": {\n            \"type\": \"string\"\n          },\n          \"ipv4\": {\n            \"type\": \"string\"\n          },\n          \"port\": {\n            \"type\": \"integer\"\n          }\n        }\n      },\n      \"remoteEndpoint\": {\n        \"type\": \"object\",\n        \"example\": {\n          \"serviceName\": \"myService\",\n          \"ipv4\"\
  : \"example_string\",\n          \"port\": 8080\n        },\n        \"properties\": {\n          \"serviceName\": {\n            \"type\": \"string\"\n          },\n          \"ipv4\": {\n            \"type\": \"string\"\n          },\n          \"port\": {\n            \"type\": \"integer\"\n          }\n        }\n      },\n      \"tags\": {\n        \"type\": \"object\",\n        \"example\": {\n          \"customAttribute\": \"example_value\"\n        }\n      },\n      \"annotations\": {\n        \"type\": \"array\",\n        \"example\": [\n          {\n            \"timestamp\": 1718153645993,\n            \"value\": \"example_string\"\n          }\n        ],\n        \"items\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"timestamp\": {\n              \"type\": \"integer\"\n            },\n            \"value\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"required\": [\n      \"id\",\n\
  \      \"traceId\"\n    ]\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ZipkinTracePayload\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-trace-zipkin-trace-payload-schema.json
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
title: ZipkinTracePayload
---
