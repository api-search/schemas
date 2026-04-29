---
description: Paginated list of test runs
layout: schema
name: TestRunList
properties_list:
- description: Total number of test runs
  name: total
  type: integer
- description: Current page number
  name: page
  type: integer
- description: Number of items per page
  name: pageSize
  type: integer
- description: Array of test run objects
  name: runs
  type: array
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
schema_file: json-schema/acceptance-criteria-management-test-run-list-schema.json
slug: acceptance-criteria-management-test-run-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.example.com/schemas/test-run-list.json\",\n  \"title\": \"TestRunList\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of test runs\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of test runs\"\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of items per page\"\n    },\n    \"runs\": {\n      \"type\": \"array\",\n      \"description\": \"Array of test run objects\",\n      \"items\": {\n        \"$ref\": \"test-run.json\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/json-schema/acceptance-criteria-management-test-run-list-schema.json
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
title: TestRunList
---
