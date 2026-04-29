---
description: Request body for creating and triggering a test run
layout: schema
name: CreateTestRunRequest
properties_list:
- description: User story IDs to test (all scenarios for these stories)
  name: storyIds
  type: array
- description: Specific scenario IDs to execute
  name: scenarioIds
  type: array
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
schema_file: json-schema/acceptance-criteria-management-create-test-run-request-schema.json
slug: acceptance-criteria-management-create-test-run-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.example.com/schemas/create-test-run-request.json\",\n  \"title\": \"CreateTestRunRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating and triggering a test run\",\n  \"properties\": {\n    \"storyIds\": {\n      \"type\": \"array\",\n      \"description\": \"User story IDs to test (all scenarios for these stories)\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"scenarioIds\": {\n      \"type\": \"array\",\n      \"description\": \"Specific scenario IDs to execute\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/json-schema/acceptance-criteria-management-create-test-run-request-schema.json
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
title: CreateTestRunRequest
---
