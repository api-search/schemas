---
description: Request body for adding an acceptance criterion to a story
layout: schema
name: CreateAcceptanceCriterionRequest
properties_list:
- description: Plain-language description of the acceptance condition
  name: description
  type: string
- description: Format of the criterion
  name: format
  type: string
- description: Gherkin Given clause
  name: given
  type: string
- description: Gherkin When clause
  name: when
  type: string
- description: Gherkin Then clause
  name: then
  type: string
- description: Display order position
  name: order
  type: integer
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
schema_file: json-schema/acceptance-criteria-management-create-acceptance-criterion-request-schema.json
slug: acceptance-criteria-management-create-acceptance-criterion-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.example.com/schemas/create-acceptance-criterion-request.json\",\n  \"title\": \"CreateAcceptanceCriterionRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for adding an acceptance criterion to a story\",\n  \"required\": [\n    \"description\"\n  ],\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Plain-language description of the acceptance condition\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"Format of the criterion\",\n      \"enum\": [\n        \"plain-text\",\n        \"gherkin\",\n        \"checklist\"\n      ]\n    },\n    \"given\": {\n      \"type\": \"string\",\n      \"description\": \"Gherkin Given clause\"\n    },\n    \"when\": {\n      \"type\": \"string\",\n      \"description\": \"Gherkin When clause\"\n    },\n    \"then\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Gherkin Then clause\"\n    },\n    \"order\": {\n      \"type\": \"integer\",\n      \"description\": \"Display order position\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/json-schema/acceptance-criteria-management-create-acceptance-criterion-request-schema.json
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
title: CreateAcceptanceCriterionRequest
---
