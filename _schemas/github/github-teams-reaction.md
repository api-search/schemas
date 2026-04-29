---
description: Reactions to conversations provide a way to help people express their feelings more simply and effectively.
layout: schema
name: reaction
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: ''
  name: user
  type: object
- description: The reaction to use
  name: content
  type: string
- description: ''
  name: created_at
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-teams-reaction-schema.json
slug: github-teams-reaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-teams-reaction-schema.json\",\n  \"title\": \"reaction\",\n  \"description\": \"Reactions to conversations provide a way to help people express their feelings more simply and effectively.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDg6UmVhY3Rpb24x\"\n    },\n    \"user\": {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\n    },\n    \"content\": {\n      \"description\": \"The reaction to use\",\n      \"example\": \"heart\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"+1\",\n        \"-1\",\n        \"laugh\",\n        \"confused\",\n        \"heart\",\n        \"hooray\",\n        \"rocket\",\n        \"eyes\"\n      ]\n \
  \   },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2016-05-20T20:09:31Z\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"node_id\",\n    \"user\",\n    \"content\",\n    \"created_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-teams-reaction-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: reaction
---
