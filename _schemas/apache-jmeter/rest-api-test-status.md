---
description: Current test status
layout: schema
name: TestStatus
properties_list:
- description: ''
  name: testId
  type: string
- description: ''
  name: status
  type: string
- description: Number of active virtual user threads
  name: activeThreads
  type: integer
- description: Elapsed test time in milliseconds
  name: elapsedTime
  type: integer
- description: Current throughput in requests per second
  name: throughput
  type: number
- description: Current error rate percentage
  name: errorRate
  type: number
provider_name: Apache JMeter
provider_slug: apache-jmeter
schema_file: json-schema/rest-api-test-status-schema.json
slug: rest-api-test-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-jmeter/refs/heads/main/json-schema/rest-api-test-status-schema.json\",\n  \"title\": \"TestStatus\",\n  \"description\": \"Current test status\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"testId\": {\n      \"type\": \"string\",\n      \"example\": \"test-1234\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"idle\",\n        \"running\",\n        \"stopping\",\n        \"stopped\"\n      ],\n      \"example\": \"running\"\n    },\n    \"activeThreads\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of active virtual user threads\",\n      \"example\": 100\n    },\n    \"elapsedTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Elapsed test time in milliseconds\",\n      \"example\": 30000\n    },\n    \"throughput\": {\n      \"type\": \"number\",\n      \"\
  description\": \"Current throughput in requests per second\",\n      \"example\": 150.5\n    },\n    \"errorRate\": {\n      \"type\": \"number\",\n      \"description\": \"Current error rate percentage\",\n      \"example\": 0.5\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-jmeter/refs/heads/main/json-schema/rest-api-test-status-schema.json
tags:
- API Testing
- Java
- Load Testing
- Open Source
- Performance Testing
- Stress Testing
title: TestStatus
---
