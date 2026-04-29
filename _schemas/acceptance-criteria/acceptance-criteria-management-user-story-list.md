---
description: Paginated list of user stories
layout: schema
name: UserStoryList
properties_list:
- description: Total number of user stories matching the query
  name: total
  type: integer
- description: Current page number
  name: page
  type: integer
- description: Number of items per page
  name: pageSize
  type: integer
- description: Array of user story objects
  name: stories
  type: array
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
schema_file: json-schema/acceptance-criteria-management-user-story-list-schema.json
slug: acceptance-criteria-management-user-story-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.example.com/schemas/user-story-list.json\",\n  \"title\": \"UserStoryList\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of user stories\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of user stories matching the query\"\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of items per page\"\n    },\n    \"stories\": {\n      \"type\": \"array\",\n      \"description\": \"Array of user story objects\",\n      \"items\": {\n        \"$ref\": \"user-story.json\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/json-schema/acceptance-criteria-management-user-story-list-schema.json
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
title: UserStoryList
---
