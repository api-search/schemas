---
description: A Gherkin BDD scenario that automates verification of an acceptance criterion
layout: schema
name: Scenario
properties_list:
- description: Unique identifier for the scenario
  name: id
  type: string
- description: ID of the parent user story
  name: storyId
  type: string
- description: ID of the linked acceptance criterion
  name: criterionId
  type: string
- description: Scenario title as it appears in the feature file
  name: title
  type: string
- description: Path to the Gherkin feature file containing this scenario
  name: featureFile
  type: string
- description: Full Gherkin text of the scenario including Given/When/Then steps
  name: gherkin
  type: string
- description: Latest test execution status
  name: status
  type: string
- description: Timestamp of the most recent test execution
  name: lastRunAt
  type: string
- description: Timestamp when the scenario was created
  name: createdAt
  type: string
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
schema_file: json-schema/acceptance-criteria-management-scenario-schema.json
slug: acceptance-criteria-management-scenario
source_filename: acceptance-criteria-management-scenario-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.example.com/schemas/scenario.json\",\n  \"title\": \"Scenario\",\n  \"type\": \"object\",\n  \"description\": \"A Gherkin BDD scenario that automates verification of an acceptance criterion\",\n  \"required\": [\n    \"id\",\n    \"title\",\n    \"featureFile\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the scenario\"\n    },\n    \"storyId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the parent user story\"\n    },\n    \"criterionId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the linked acceptance criterion\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Scenario title as it appears in the feature file\"\n    },\n    \"featureFile\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the Gherkin feature file containing\
  \ this scenario\"\n    },\n    \"gherkin\": {\n      \"type\": \"string\",\n      \"description\": \"Full Gherkin text of the scenario including Given/When/Then steps\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Latest test execution status\",\n      \"enum\": [\n        \"pending\",\n        \"passing\",\n        \"failing\",\n        \"skipped\"\n      ]\n    },\n    \"lastRunAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent test execution\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the scenario was created\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/json-schema/acceptance-criteria-management-scenario-schema.json
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
title: Scenario
---
