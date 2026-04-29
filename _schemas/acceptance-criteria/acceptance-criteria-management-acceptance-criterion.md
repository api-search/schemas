---
description: A single testable condition that must be met for a user story to be accepted as complete
layout: schema
name: AcceptanceCriterion
properties_list:
- description: Unique identifier for the acceptance criterion
  name: id
  type: string
- description: ID of the parent user story
  name: storyId
  type: string
- description: Plain-language description of the acceptance condition
  name: description
  type: string
- description: Format used to express the criterion
  name: format
  type: string
- description: Gherkin Given clause (context/precondition) if format is gherkin
  name: given
  type: string
- description: Gherkin When clause (action/trigger) if format is gherkin
  name: when
  type: string
- description: Gherkin Then clause (expected outcome) if format is gherkin
  name: then
  type: string
- description: Verification status of this criterion
  name: status
  type: string
- description: Display order position within the parent story
  name: order
  type: integer
- description: Timestamp when the criterion was created
  name: createdAt
  type: string
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
schema_file: json-schema/acceptance-criteria-management-acceptance-criterion-schema.json
slug: acceptance-criteria-management-acceptance-criterion
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.example.com/schemas/acceptance-criterion.json\",\n  \"title\": \"AcceptanceCriterion\",\n  \"type\": \"object\",\n  \"description\": \"A single testable condition that must be met for a user story to be accepted as complete\",\n  \"required\": [\n    \"id\",\n    \"description\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the acceptance criterion\"\n    },\n    \"storyId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the parent user story\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Plain-language description of the acceptance condition\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"Format used to express the criterion\",\n      \"enum\": [\n        \"plain-text\",\n        \"gherkin\",\n        \"checklist\"\n\
  \      ]\n    },\n    \"given\": {\n      \"type\": \"string\",\n      \"description\": \"Gherkin Given clause (context/precondition) if format is gherkin\"\n    },\n    \"when\": {\n      \"type\": \"string\",\n      \"description\": \"Gherkin When clause (action/trigger) if format is gherkin\"\n    },\n    \"then\": {\n      \"type\": \"string\",\n      \"description\": \"Gherkin Then clause (expected outcome) if format is gherkin\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Verification status of this criterion\",\n      \"enum\": [\n        \"not-verified\",\n        \"passing\",\n        \"failing\"\n      ]\n    },\n    \"order\": {\n      \"type\": \"integer\",\n      \"description\": \"Display order position within the parent story\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the criterion was created\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/json-schema/acceptance-criteria-management-acceptance-criterion-schema.json
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
title: AcceptanceCriterion
---
