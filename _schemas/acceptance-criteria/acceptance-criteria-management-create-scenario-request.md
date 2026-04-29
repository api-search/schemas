---
description: Request body for creating a BDD scenario
layout: schema
name: CreateScenarioRequest
properties_list:
- description: ID of the parent user story
  name: storyId
  type: string
- description: ID of the linked acceptance criterion
  name: criterionId
  type: string
- description: Scenario title
  name: title
  type: string
- description: Feature file path
  name: featureFile
  type: string
- description: Full Gherkin scenario text
  name: gherkin
  type: string
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
schema_file: json-schema/acceptance-criteria-management-create-scenario-request-schema.json
slug: acceptance-criteria-management-create-scenario-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.example.com/schemas/create-scenario-request.json\",\n  \"title\": \"CreateScenarioRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a BDD scenario\",\n  \"required\": [\n    \"storyId\",\n    \"title\",\n    \"featureFile\",\n    \"gherkin\"\n  ],\n  \"properties\": {\n    \"storyId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the parent user story\"\n    },\n    \"criterionId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the linked acceptance criterion\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Scenario title\"\n    },\n    \"featureFile\": {\n      \"type\": \"string\",\n      \"description\": \"Feature file path\"\n    },\n    \"gherkin\": {\n      \"type\": \"string\",\n      \"description\": \"Full Gherkin scenario text\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/json-schema/acceptance-criteria-management-create-scenario-request-schema.json
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
title: CreateScenarioRequest
---
