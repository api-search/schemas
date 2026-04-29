---
description: Paginated list of quizzes
layout: schema
name: QuizList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: total
  type: integer
- description: ''
  name: page
  type: integer
- description: ''
  name: limit
  type: integer
provider_name: Acadia
provider_slug: acadia
schema_file: json-schema/acadia-quiz-list-schema.json
slug: acadia-quiz-list
source_filename: acadia-quiz-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-quiz-list-schema.json\",\n  \"title\": \"QuizList\",\n  \"description\": \"Paginated list of quizzes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Quiz\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 15\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"example\": 25\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-quiz-list-schema.json
tags:
- Connected Worker
- Knowledge Management
- Manufacturing
- Skills Management
- Training
- Workforce Development
title: QuizList
---
