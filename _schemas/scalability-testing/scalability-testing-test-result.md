---
description: Schema for aggregated results from a load or scalability test run
layout: schema
name: LoadTestResult
properties_list:
- description: Unique identifier for this test run
  name: testRunId
  type: string
- description: Name of the load test scenario
  name: testName
  type: string
- description: Load testing tool used to execute the test
  name: tool
  type: string
- description: ISO 8601 timestamp when the test started
  name: startTime
  type: string
- description: ISO 8601 timestamp when the test completed
  name: endTime
  type: string
- description: Total test duration in seconds
  name: durationSeconds
  type: integer
- description: Test configuration parameters
  name: configuration
  type: object
- description: Aggregated performance metrics from the test run
  name: metrics
  type: object
- description: List of service-level agreement thresholds that were violated
  name: slaViolations
  type: array
- description: Whether the test passed all configured SLA thresholds
  name: passed
  type: boolean
provider_name: Scalability Testing
provider_slug: scalability-testing
schema_file: json-schema/scalability-testing-test-result-schema.json
slug: scalability-testing-test-result
source_filename: scalability-testing-test-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scalability-testing/main/json-schema/scalability-testing-test-result-schema.json\",\n  \"title\": \"LoadTestResult\",\n  \"description\": \"Schema for aggregated results from a load or scalability test run\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"testRunId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this test run\",\n      \"example\": \"run_20260502_001\"\n    },\n    \"testName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the load test scenario\",\n      \"example\": \"API Gateway Peak Load Test\"\n    },\n    \"tool\": {\n      \"type\": \"string\",\n      \"description\": \"Load testing tool used to execute the test\",\n      \"enum\": [\"JMeter\", \"k6\", \"Gatling\", \"Locust\", \"Artillery\", \"Vegeta\", \"Wrk\", \"Azure Load Testing\", \"BlazeMeter\"],\n      \"\
  example\": \"k6\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the test started\",\n      \"example\": \"2026-05-02T10:00:00.000Z\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the test completed\",\n      \"example\": \"2026-05-02T10:30:00.000Z\"\n    },\n    \"durationSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Total test duration in seconds\",\n      \"minimum\": 1,\n      \"example\": 1800\n    },\n    \"configuration\": {\n      \"type\": \"object\",\n      \"description\": \"Test configuration parameters\",\n      \"properties\": {\n        \"virtualUsers\": {\n          \"type\": \"integer\",\n          \"description\": \"Peak number of concurrent virtual users (VUs) simulated\",\n          \"minimum\": 1,\n          \"example\": 1000\n        },\n        \"rampUpSeconds\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"Time in seconds to ramp up to peak virtual users\",\n          \"example\": 300\n        },\n        \"targetUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Base URL of the system under test\",\n          \"example\": \"https://api.example.com\"\n        },\n        \"testType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of scalability/performance test\",\n          \"enum\": [\"Load Test\", \"Stress Test\", \"Spike Test\", \"Soak Test\", \"Capacity Test\", \"Breakpoint Test\"],\n          \"example\": \"Load Test\"\n        }\n      }\n    },\n    \"metrics\": {\n      \"type\": \"object\",\n      \"description\": \"Aggregated performance metrics from the test run\",\n      \"properties\": {\n        \"totalRequests\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of HTTP requests made during the test\"\
  ,\n          \"example\": 540000\n        },\n        \"requestsPerSecond\": {\n          \"type\": \"number\",\n          \"description\": \"Average requests per second (throughput)\",\n          \"example\": 300.0\n        },\n        \"responseTime\": {\n          \"type\": \"object\",\n          \"description\": \"Response time statistics in milliseconds\",\n          \"properties\": {\n            \"min\": {\"type\": \"number\", \"description\": \"Minimum response time (ms)\"},\n            \"max\": {\"type\": \"number\", \"description\": \"Maximum response time (ms)\"},\n            \"mean\": {\"type\": \"number\", \"description\": \"Mean (average) response time (ms)\"},\n            \"median\": {\"type\": \"number\", \"description\": \"50th percentile response time (ms)\"},\n            \"p90\": {\"type\": \"number\", \"description\": \"90th percentile response time (ms)\"},\n            \"p95\": {\"type\": \"number\", \"description\": \"95th percentile response time (ms)\"},\n\
  \            \"p99\": {\"type\": \"number\", \"description\": \"99th percentile response time (ms)\"}\n          }\n        },\n        \"errorRate\": {\n          \"type\": \"number\",\n          \"description\": \"Percentage of requests that resulted in errors (4xx/5xx)\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"example\": 0.5\n        },\n        \"errorCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of error responses during the test\",\n          \"example\": 2700\n        },\n        \"apdex\": {\n          \"type\": \"number\",\n          \"description\": \"Application Performance Index score (0.0-1.0). Based on configurable satisfied/tolerating thresholds.\",\n          \"minimum\": 0,\n          \"maximum\": 1,\n          \"example\": 0.87\n        },\n        \"bandwidthMbps\": {\n          \"type\": \"number\",\n          \"description\": \"Average network bandwidth consumed (Mbps)\",\n          \"example\"\
  : 45.2\n        }\n      }\n    },\n    \"slaViolations\": {\n      \"type\": \"array\",\n      \"description\": \"List of service-level agreement thresholds that were violated\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"metric\": {\"type\": \"string\", \"description\": \"Metric name (e.g., p95_response_time)\"},\n          \"threshold\": {\"type\": \"number\", \"description\": \"SLA threshold value\"},\n          \"actual\": {\"type\": \"number\", \"description\": \"Actual measured value\"},\n          \"unit\": {\"type\": \"string\", \"description\": \"Unit of measurement\"}\n        }\n      }\n    },\n    \"passed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the test passed all configured SLA thresholds\",\n      \"example\": true\n    }\n  },\n  \"required\": [\"testRunId\", \"testName\", \"tool\", \"startTime\", \"durationSeconds\", \"configuration\", \"metrics\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalability-testing/refs/heads/main/json-schema/scalability-testing-test-result-schema.json
tags:
- API Testing
- Load Testing
- Performance Testing
- Scalability
- Stress Testing
title: LoadTestResult
---
