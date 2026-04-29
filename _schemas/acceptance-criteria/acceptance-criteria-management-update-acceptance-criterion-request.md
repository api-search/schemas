---
description: Request body for updating an acceptance criterion
layout: schema
name: UpdateAcceptanceCriterionRequest
properties_list:
- description: Updated description
  name: description
  type: string
- description: Updated Given clause
  name: given
  type: string
- description: Updated When clause
  name: when
  type: string
- description: Updated Then clause
  name: then
  type: string
- description: Updated verification status
  name: status
  type: string
- description: Updated display order
  name: order
  type: integer
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
schema_file: json-schema/acceptance-criteria-management-update-acceptance-criterion-request-schema.json
slug: acceptance-criteria-management-update-acceptance-criterion-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.example.com/schemas/update-acceptance-criterion-request.json\",\n  \"title\": \"UpdateAcceptanceCriterionRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating an acceptance criterion\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Updated description\"\n    },\n    \"given\": {\n      \"type\": \"string\",\n      \"description\": \"Updated Given clause\"\n    },\n    \"when\": {\n      \"type\": \"string\",\n      \"description\": \"Updated When clause\"\n    },\n    \"then\": {\n      \"type\": \"string\",\n      \"description\": \"Updated Then clause\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Updated verification status\",\n      \"enum\": [\n        \"not-verified\",\n        \"passing\",\n        \"failing\"\n      ]\n    },\n    \"order\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Updated display order\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/json-schema/acceptance-criteria-management-update-acceptance-criterion-request-schema.json
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
title: UpdateAcceptanceCriterionRequest
---
