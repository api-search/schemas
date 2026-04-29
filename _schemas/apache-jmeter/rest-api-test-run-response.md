---
description: Response from starting a test
layout: schema
name: TestRunResponse
properties_list:
- description: Unique test run identifier
  name: testId
  type: string
- description: ''
  name: status
  type: string
- description: Test start timestamp
  name: startTime
  type: integer
provider_name: Apache JMeter
provider_slug: apache-jmeter
schema_file: json-schema/rest-api-test-run-response-schema.json
slug: rest-api-test-run-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-jmeter/refs/heads/main/json-schema/rest-api-test-run-response-schema.json\",\n  \"title\": \"TestRunResponse\",\n  \"description\": \"Response from starting a test\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"testId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique test run identifier\",\n      \"example\": \"test-1234\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"running\"\n    },\n    \"startTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Test start timestamp\",\n      \"example\": 1718153645993\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-jmeter/refs/heads/main/json-schema/rest-api-test-run-response-schema.json
tags:
- API Testing
- Java
- Load Testing
- Open Source
- Performance Testing
- Stress Testing
title: TestRunResponse
---
