---
description: A user story representing a feature or requirement from the perspective of an end user
layout: schema
name: UserStory
properties_list:
- description: Unique identifier for the user story
  name: id
  type: string
- description: Short title summarizing the user story (As a... I want... So that...)
  name: title
  type: string
- description: Full user story narrative including role, goal, and benefit
  name: description
  type: string
- description: Current lifecycle status of the user story
  name: status
  type: string
- description: Priority level of the user story
  name: priority
  type: string
- description: Effort estimate in story points
  name: storyPoints
  type: integer
- description: List of acceptance criteria that define done for this story
  name: acceptanceCriteria
  type: array
- description: Labels or tags associated with the story
  name: tags
  type: array
- description: Username or ID of the person assigned to this story
  name: assignee
  type: string
- description: Timestamp when the user story was created
  name: createdAt
  type: string
- description: Timestamp when the user story was last updated
  name: updatedAt
  type: string
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
schema_file: json-schema/acceptance-criteria-management-user-story-schema.json
slug: acceptance-criteria-management-user-story
source_filename: acceptance-criteria-management-user-story-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.example.com/schemas/user-story.json\",\n  \"title\": \"UserStory\",\n  \"type\": \"object\",\n  \"description\": \"A user story representing a feature or requirement from the perspective of an end user\",\n  \"required\": [\n    \"id\",\n    \"title\",\n    \"status\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user story\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Short title summarizing the user story (As a... I want... So that...)\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Full user story narrative including role, goal, and benefit\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the user story\",\n      \"enum\": [\n        \"backlog\",\n        \"in-progress\"\
  ,\n        \"ready-for-review\",\n        \"done\"\n      ]\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"Priority level of the user story\",\n      \"enum\": [\n        \"low\",\n        \"medium\",\n        \"high\",\n        \"critical\"\n      ]\n    },\n    \"storyPoints\": {\n      \"type\": \"integer\",\n      \"description\": \"Effort estimate in story points\"\n    },\n    \"acceptanceCriteria\": {\n      \"type\": \"array\",\n      \"description\": \"List of acceptance criteria that define done for this story\",\n      \"items\": {\n        \"$ref\": \"acceptance-criterion.json\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Labels or tags associated with the story\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"assignee\": {\n      \"type\": \"string\",\n      \"description\": \"Username or ID of the person assigned to this story\"\n    },\n    \"createdAt\": {\n    \
  \  \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the user story was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the user story was last updated\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/json-schema/acceptance-criteria-management-user-story-schema.json
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
title: UserStory
---
