---
description: JSON representation of a JUnit-style test report (testsuites/testsuite/testcase).
layout: schema
name: JUnit Test Report
properties_list:
- description: ''
  name: testsuites
  type: object
provider_name: JUnit
provider_slug: junit
schema_file: json-schema/junit-report-schema.json
slug: junit-report
source_filename: junit-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/junit/main/json-schema/junit-report-schema.json\",\n  \"title\": \"JUnit Test Report\",\n  \"description\": \"JSON representation of a JUnit-style test report (testsuites/testsuite/testcase).\",\n  \"type\": \"object\",\n  \"required\": [\"testsuites\"],\n  \"properties\": {\n    \"testsuites\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": { \"type\": \"string\" },\n        \"tests\": { \"type\": \"integer\", \"minimum\": 0 },\n        \"failures\": { \"type\": \"integer\", \"minimum\": 0 },\n        \"errors\": { \"type\": \"integer\", \"minimum\": 0 },\n        \"skipped\": { \"type\": \"integer\", \"minimum\": 0 },\n        \"time\": { \"type\": \"number\", \"minimum\": 0 },\n        \"testsuite\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"required\"\
  : [\"name\", \"tests\"],\n            \"properties\": {\n              \"name\": { \"type\": \"string\" },\n              \"package\": { \"type\": \"string\" },\n              \"tests\": { \"type\": \"integer\", \"minimum\": 0 },\n              \"failures\": { \"type\": \"integer\", \"minimum\": 0 },\n              \"errors\": { \"type\": \"integer\", \"minimum\": 0 },\n              \"skipped\": { \"type\": \"integer\", \"minimum\": 0 },\n              \"time\": { \"type\": \"number\", \"minimum\": 0 },\n              \"timestamp\": { \"type\": \"string\", \"format\": \"date-time\" },\n              \"hostname\": { \"type\": \"string\" },\n              \"properties\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"name\": { \"type\": \"string\" },\n                    \"value\": { \"type\": \"string\" }\n                  }\n                }\n              },\n\
  \              \"testcase\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"required\": [\"name\"],\n                  \"properties\": {\n                    \"name\": { \"type\": \"string\" },\n                    \"classname\": { \"type\": \"string\" },\n                    \"time\": { \"type\": \"number\", \"minimum\": 0 },\n                    \"skipped\": {\n                      \"type\": \"object\",\n                      \"properties\": { \"message\": { \"type\": \"string\" } }\n                    },\n                    \"failure\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"message\": { \"type\": \"string\" },\n                        \"type\": { \"type\": \"string\" },\n                        \"text\": { \"type\": \"string\" }\n                      }\n                    },\n                    \"error\": {\n        \
  \              \"type\": \"object\",\n                      \"properties\": {\n                        \"message\": { \"type\": \"string\" },\n                        \"type\": { \"type\": \"string\" },\n                        \"text\": { \"type\": \"string\" }\n                      }\n                    },\n                    \"system-out\": { \"type\": \"string\" },\n                    \"system-err\": { \"type\": \"string\" }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/junit/refs/heads/main/json-schema/junit-report-schema.json
tags:
- Java
- TDD
- Test Automation
- Testing
- Unit Testing
title: JUnit Test Report
---
