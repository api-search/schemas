---
description: Request to start a JMeter test
layout: schema
name: TestRunRequest
properties_list:
- description: Path to the JMeter test plan file
  name: testPlan
  type: string
- description: JMeter properties to override
  name: properties
  type: object
provider_name: Apache JMeter
provider_slug: apache-jmeter
schema_file: json-schema/rest-api-test-run-request-schema.json
slug: rest-api-test-run-request
source_filename: rest-api-test-run-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-jmeter/refs/heads/main/json-schema/rest-api-test-run-request-schema.json\",\n  \"title\": \"TestRunRequest\",\n  \"description\": \"Request to start a JMeter test\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"testPlan\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the JMeter test plan file\",\n      \"example\": \"/tests/my-load-test.jmx\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"JMeter properties to override\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-jmeter/refs/heads/main/json-schema/rest-api-test-run-request-schema.json
tags:
- API Testing
- Java
- Load Testing
- Open Source
- Performance Testing
- Stress Testing
title: TestRunRequest
---
