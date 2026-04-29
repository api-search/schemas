---
description: Paginated list of BDD scenarios
layout: schema
name: ScenarioList
properties_list:
- description: Total number of scenarios matching the query
  name: total
  type: integer
- description: Current page number
  name: page
  type: integer
- description: Number of items per page
  name: pageSize
  type: integer
- description: Array of scenario objects
  name: scenarios
  type: array
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
schema_file: json-schema/acceptance-criteria-management-scenario-list-schema.json
slug: acceptance-criteria-management-scenario-list
source_filename: acceptance-criteria-management-scenario-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.example.com/schemas/scenario-list.json\",\n  \"title\": \"ScenarioList\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of BDD scenarios\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of scenarios matching the query\"\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of items per page\"\n    },\n    \"scenarios\": {\n      \"type\": \"array\",\n      \"description\": \"Array of scenario objects\",\n      \"items\": {\n        \"$ref\": \"scenario.json\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/json-schema/acceptance-criteria-management-scenario-list-schema.json
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
title: ScenarioList
---
