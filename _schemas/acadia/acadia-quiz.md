---
description: A quiz or assessment
layout: schema
name: Quiz
properties_list:
- description: Quiz identifier
  name: id
  type: string
- description: Quiz title
  name: title
  type: string
- description: Quiz status
  name: status
  type: string
- description: Number of questions in the quiz
  name: questionCount
  type: integer
- description: Minimum passing score percentage
  name: passingScore
  type: integer
- description: Quiz creation timestamp
  name: createdAt
  type: string
provider_name: Acadia
provider_slug: acadia
schema_file: json-schema/acadia-quiz-schema.json
slug: acadia-quiz
source_filename: acadia-quiz-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-quiz-schema.json\",\n  \"title\": \"Quiz\",\n  \"description\": \"A quiz or assessment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Quiz identifier\",\n      \"example\": \"quiz-jkl012\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Quiz title\",\n      \"example\": \"Machine Safety Knowledge Check\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Quiz status\",\n      \"example\": \"active\",\n      \"enum\": [\n        \"active\",\n        \"inactive\"\n      ]\n    },\n    \"questionCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of questions in the quiz\",\n      \"example\": 10\n    },\n    \"passingScore\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Minimum passing score percentage\",\n      \"example\": 80\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Quiz creation timestamp\",\n      \"example\": \"2026-01-20T10:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-quiz-schema.json
tags:
- Connected Worker
- Knowledge Management
- Manufacturing
- Skills Management
- Training
- Workforce Development
title: Quiz
---
