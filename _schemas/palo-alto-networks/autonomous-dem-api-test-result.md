---
description: TestResult schema from Palo Alto Networks Autonomous DEM API
layout: schema
name: TestResult
properties_list:
- description: Timestamp of the test execution.
  name: timestamp
  type: string
- description: Synthetic test identifier.
  name: test_id
  type: string
- description: Agent that ran the test.
  name: agent_id
  type: string
- description: User associated with the agent.
  name: user_id
  type: string
- description: Test execution result status.
  name: status
  type: string
- description: Total response latency in milliseconds.
  name: latency_ms
  type: number
- description: DNS resolution time in milliseconds.
  name: dns_time_ms
  type: number
- description: TCP connection establishment time in milliseconds.
  name: tcp_connect_ms
  type: number
- description: Time to first byte for HTTP tests in milliseconds.
  name: ttfb_ms
  type: number
- description: HTTP response status code for HTTP type tests.
  name: http_status_code
  type: integer
- description: Error message if the test failed.
  name: error_message
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/autonomous-dem-api-test-result-schema.json
slug: autonomous-dem-api-test-result
source_filename: autonomous-dem-api-test-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TestResult\",\n  \"description\": \"TestResult schema from Palo Alto Networks Autonomous DEM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/autonomous-dem-api-test-result-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the test execution.\"\n    },\n    \"test_id\": {\n      \"type\": \"string\",\n      \"description\": \"Synthetic test identifier.\"\n    },\n    \"agent_id\": {\n      \"type\": \"string\",\n      \"description\": \"Agent that ran the test.\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"User associated with the agent.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"success\",\n        \"failure\"\
  ,\n        \"timeout\"\n      ],\n      \"description\": \"Test execution result status.\"\n    },\n    \"latency_ms\": {\n      \"type\": \"number\",\n      \"description\": \"Total response latency in milliseconds.\"\n    },\n    \"dns_time_ms\": {\n      \"type\": \"number\",\n      \"description\": \"DNS resolution time in milliseconds.\"\n    },\n    \"tcp_connect_ms\": {\n      \"type\": \"number\",\n      \"description\": \"TCP connection establishment time in milliseconds.\"\n    },\n    \"ttfb_ms\": {\n      \"type\": \"number\",\n      \"description\": \"Time to first byte for HTTP tests in milliseconds.\"\n    },\n    \"http_status_code\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP response status code for HTTP type tests.\"\n    },\n    \"error_message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message if the test failed.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/autonomous-dem-api-test-result-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: TestResult
---
