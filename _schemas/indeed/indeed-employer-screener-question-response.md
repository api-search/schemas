---
description: A candidate's response to a screener question on the job posting.
layout: schema
name: ScreenerQuestionResponse
properties_list:
- description: The unique identifier of the screener question.
  name: questionId
  type: string
- description: The text of the screener question.
  name: question
  type: string
- description: The candidate's answer to the question.
  name: answer
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-screener-question-response-schema.json
slug: indeed-employer-screener-question-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScreenerQuestionResponse\",\n  \"type\": \"object\",\n  \"description\": \"A candidate's response to a screener question on the job posting.\",\n  \"properties\": {\n    \"questionId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the screener question.\"\n    },\n    \"question\": {\n      \"type\": \"string\",\n      \"description\": \"The text of the screener question.\"\n    },\n    \"answer\": {\n      \"type\": \"string\",\n      \"description\": \"The candidate's answer to the question.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-screener-question-response-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: ScreenerQuestionResponse
---
