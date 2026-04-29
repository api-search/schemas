---
description: Request body for updating an existing user story
layout: schema
name: UpdateUserStoryRequest
properties_list:
- description: Updated title
  name: title
  type: string
- description: Updated description
  name: description
  type: string
- description: Updated status
  name: status
  type: string
- description: Updated priority
  name: priority
  type: string
- description: Updated story point estimate
  name: storyPoints
  type: integer
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
schema_file: json-schema/acceptance-criteria-management-update-user-story-request-schema.json
slug: acceptance-criteria-management-update-user-story-request
source_filename: acceptance-criteria-management-update-user-story-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.example.com/schemas/update-user-story-request.json\",\n  \"title\": \"UpdateUserStoryRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating an existing user story\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Updated title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Updated description\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Updated status\",\n      \"enum\": [\n        \"backlog\",\n        \"in-progress\",\n        \"ready-for-review\",\n        \"done\"\n      ]\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"Updated priority\",\n      \"enum\": [\n        \"low\",\n        \"medium\",\n        \"high\",\n        \"critical\"\n      ]\n    },\n    \"storyPoints\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Updated story point estimate\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/json-schema/acceptance-criteria-management-update-user-story-request-schema.json
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
title: UpdateUserStoryRequest
---
