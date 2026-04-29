---
description: Request body for creating a new user story
layout: schema
name: CreateUserStoryRequest
properties_list:
- description: Short title for the user story
  name: title
  type: string
- description: Full user story narrative
  name: description
  type: string
- description: Priority level
  name: priority
  type: string
- description: Effort estimate in story points
  name: storyPoints
  type: integer
- description: Labels or tags
  name: tags
  type: array
- description: Assignee username or ID
  name: assignee
  type: string
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
schema_file: json-schema/acceptance-criteria-management-create-user-story-request-schema.json
slug: acceptance-criteria-management-create-user-story-request
source_filename: acceptance-criteria-management-create-user-story-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.example.com/schemas/create-user-story-request.json\",\n  \"title\": \"CreateUserStoryRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new user story\",\n  \"required\": [\n    \"title\"\n  ],\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Short title for the user story\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Full user story narrative\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"Priority level\",\n      \"enum\": [\n        \"low\",\n        \"medium\",\n        \"high\",\n        \"critical\"\n      ]\n    },\n    \"storyPoints\": {\n      \"type\": \"integer\",\n      \"description\": \"Effort estimate in story points\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Labels or tags\"\
  ,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"assignee\": {\n      \"type\": \"string\",\n      \"description\": \"Assignee username or ID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/json-schema/acceptance-criteria-management-create-user-story-request-schema.json
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
title: CreateUserStoryRequest
---
