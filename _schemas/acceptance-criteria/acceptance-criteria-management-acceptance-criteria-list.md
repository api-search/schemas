---
description: List of acceptance criteria for a user story
layout: schema
name: AcceptanceCriteriaList
properties_list:
- description: Total number of acceptance criteria
  name: total
  type: integer
- description: Current page number
  name: page
  type: integer
- description: Number of items per page
  name: pageSize
  type: integer
- description: Array of acceptance criteria
  name: criteria
  type: array
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
schema_file: json-schema/acceptance-criteria-management-acceptance-criteria-list-schema.json
slug: acceptance-criteria-management-acceptance-criteria-list
source_filename: acceptance-criteria-management-acceptance-criteria-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.example.com/schemas/acceptance-criteria-list.json\",\n  \"title\": \"AcceptanceCriteriaList\",\n  \"type\": \"object\",\n  \"description\": \"List of acceptance criteria for a user story\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of acceptance criteria\"\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of items per page\"\n    },\n    \"criteria\": {\n      \"type\": \"array\",\n      \"description\": \"Array of acceptance criteria\",\n      \"items\": {\n        \"$ref\": \"acceptance-criterion.json\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/json-schema/acceptance-criteria-management-acceptance-criteria-list-schema.json
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
title: AcceptanceCriteriaList
---
