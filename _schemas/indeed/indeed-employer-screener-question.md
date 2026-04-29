---
description: A screener question configured on a job posting.
layout: schema
name: ScreenerQuestion
properties_list:
- description: Unique identifier for the screener question.
  name: id
  type: string
- description: The text of the question.
  name: question
  type: string
- description: The type of expected response.
  name: type
  type: string
- description: Whether the candidate must answer this question.
  name: required
  type: boolean
- description: Available options for select-type questions.
  name: options
  type: array
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-screener-question-schema.json
slug: indeed-employer-screener-question
source_filename: indeed-employer-screener-question-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScreenerQuestion\",\n  \"type\": \"object\",\n  \"description\": \"A screener question configured on a job posting.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the screener question.\"\n    },\n    \"question\": {\n      \"type\": \"string\",\n      \"description\": \"The text of the question.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of expected response.\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the candidate must answer this question.\"\n    },\n    \"options\": {\n      \"type\": \"array\",\n      \"description\": \"Available options for select-type questions.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-screener-question-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: ScreenerQuestion
---
