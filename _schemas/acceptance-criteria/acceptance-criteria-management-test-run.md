---
description: An execution instance of acceptance criteria tests across one or more stories or scenarios
layout: schema
name: TestRun
properties_list:
- description: Unique identifier for the test run
  name: id
  type: string
- description: User story IDs included in this test run
  name: storyIds
  type: array
- description: Specific scenario IDs included in this test run
  name: scenarioIds
  type: array
- description: Overall test run status
  name: status
  type: string
- description: Total number of scenarios in this run
  name: totalScenarios
  type: integer
- description: Number of scenarios that passed
  name: passedScenarios
  type: integer
- description: Number of scenarios that failed
  name: failedScenarios
  type: integer
- description: Number of scenarios that were skipped
  name: skippedScenarios
  type: integer
- description: Timestamp when the test run started
  name: startedAt
  type: string
- description: Timestamp when the test run completed
  name: completedAt
  type: string
- description: URL to the detailed test run report
  name: reportUrl
  type: string
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
schema_file: json-schema/acceptance-criteria-management-test-run-schema.json
slug: acceptance-criteria-management-test-run
source_filename: acceptance-criteria-management-test-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.example.com/schemas/test-run.json\",\n  \"title\": \"TestRun\",\n  \"type\": \"object\",\n  \"description\": \"An execution instance of acceptance criteria tests across one or more stories or scenarios\",\n  \"required\": [\n    \"id\",\n    \"status\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the test run\"\n    },\n    \"storyIds\": {\n      \"type\": \"array\",\n      \"description\": \"User story IDs included in this test run\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"scenarioIds\": {\n      \"type\": \"array\",\n      \"description\": \"Specific scenario IDs included in this test run\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Overall test run status\",\n      \"enum\"\
  : [\n        \"queued\",\n        \"running\",\n        \"passed\",\n        \"failed\",\n        \"cancelled\"\n      ]\n    },\n    \"totalScenarios\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of scenarios in this run\"\n    },\n    \"passedScenarios\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of scenarios that passed\"\n    },\n    \"failedScenarios\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of scenarios that failed\"\n    },\n    \"skippedScenarios\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of scenarios that were skipped\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the test run started\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the test run completed\"\n    },\n    \"reportUrl\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"URL to the detailed test run report\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/json-schema/acceptance-criteria-management-test-run-schema.json
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
title: TestRun
---
