---
description: Schema for a Reflect test execution record including status and per-test results.
layout: schema
name: Reflect Test Execution
properties_list:
- description: Unique integer identifier for the execution.
  name: executionId
  type: integer
- description: Results for each test within the execution.
  name: tests
  type: array
provider_name: Reflect
provider_slug: reflect
schema_file: json-schema/reflect-execution-schema.json
slug: reflect-execution
source_filename: reflect-execution-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/reflect/json-schema/reflect-execution-schema.json\",\n  \"title\": \"Reflect Test Execution\",\n  \"description\": \"Schema for a Reflect test execution record including status and per-test results.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique integer identifier for the execution.\"\n    },\n    \"tests\": {\n      \"type\": \"array\",\n      \"description\": \"Results for each test within the execution.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"testId\": {\n            \"type\": \"integer\",\n            \"description\": \"ID of the test that was executed.\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"description\": \"Execution status of the test.\",\n            \"enum\": [\"pending\"\
  , \"running\", \"passed\", \"failed\", \"error\"]\n          },\n          \"started\": {\n            \"type\": \"integer\",\n            \"description\": \"Unix timestamp when the test execution started.\"\n          },\n          \"completed\": {\n            \"type\": \"integer\",\n            \"description\": \"Unix timestamp when the test execution completed.\"\n          }\n        },\n        \"required\": [\"testId\", \"status\"]\n      }\n    }\n  },\n  \"required\": [\"executionId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reflect/refs/heads/main/json-schema/reflect-execution-schema.json
tags:
- AI Testing
- Artificial Intelligence
- Automated Testing
- CI/CD
- End-to-End Testing
- QA
- Testing
title: Reflect Test Execution
---
