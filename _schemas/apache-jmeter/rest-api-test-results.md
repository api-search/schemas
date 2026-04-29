---
description: Test performance results
layout: schema
name: TestResults
properties_list:
- description: ''
  name: testId
  type: string
- description: ''
  name: totalRequests
  type: integer
- description: ''
  name: errorCount
  type: integer
- description: Average response time in milliseconds
  name: averageResponseTime
  type: number
- description: ''
  name: minResponseTime
  type: number
- description: ''
  name: maxResponseTime
  type: number
- description: 90th percentile response time
  name: percentile90
  type: number
- description: Average throughput in requests/second
  name: throughput
  type: number
provider_name: Apache JMeter
provider_slug: apache-jmeter
schema_file: json-schema/rest-api-test-results-schema.json
slug: rest-api-test-results
source_filename: rest-api-test-results-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-jmeter/refs/heads/main/json-schema/rest-api-test-results-schema.json\",\n  \"title\": \"TestResults\",\n  \"description\": \"Test performance results\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"testId\": {\n      \"type\": \"string\",\n      \"example\": \"test-1234\"\n    },\n    \"totalRequests\": {\n      \"type\": \"integer\",\n      \"example\": 10000\n    },\n    \"errorCount\": {\n      \"type\": \"integer\",\n      \"example\": 50\n    },\n    \"averageResponseTime\": {\n      \"type\": \"number\",\n      \"description\": \"Average response time in milliseconds\",\n      \"example\": 250.5\n    },\n    \"minResponseTime\": {\n      \"type\": \"number\",\n      \"example\": 50.0\n    },\n    \"maxResponseTime\": {\n      \"type\": \"number\",\n      \"example\": 5000.0\n    },\n    \"percentile90\": {\n      \"type\": \"\
  number\",\n      \"description\": \"90th percentile response time\",\n      \"example\": 500.0\n    },\n    \"throughput\": {\n      \"type\": \"number\",\n      \"description\": \"Average throughput in requests/second\",\n      \"example\": 148.7\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-jmeter/refs/heads/main/json-schema/rest-api-test-results-schema.json
tags:
- API Testing
- Java
- Load Testing
- Open Source
- Performance Testing
- Stress Testing
title: TestResults
---
