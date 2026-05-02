---
description: A Hotjar survey definition including its configuration, status, and questions.
layout: schema
name: Hotjar Survey
properties_list:
- description: The unique identifier for the survey.
  name: id
  type: integer
- description: The name of the survey.
  name: name
  type: string
- description: The type of survey.
  name: type
  type: string
- description: Whether the survey is currently active and collecting responses.
  name: is_enabled
  type: boolean
- description: The ISO 8601 timestamp when the survey was created.
  name: created_time
  type: string
- description: The URL path to the survey resource in the API.
  name: url
  type: string
- description: The URL path to retrieve the survey responses.
  name: responses_url
  type: string
- description: Whether sentiment analysis is enabled for this survey.
  name: sentiment_analysis_enabled
  type: boolean
- description: The list of questions in the survey.
  name: questions
  type: array
provider_name: hotjar
provider_slug: hotjar
schema_file: json-schema/hotjar-survey-schema.json
slug: hotjar-survey
source_filename: hotjar-survey-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://hotjar.com/schemas/hotjar/survey.json\",\n  \"title\": \"Hotjar Survey\",\n  \"description\": \"A Hotjar survey definition including its configuration, status, and questions.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier for the survey.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the survey.\",\n      \"minLength\": 1\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of survey.\",\n      \"enum\": [\"popover\", \"fullscreen\", \"external_link\"]\n    },\n    \"is_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the survey is currently active and collecting responses.\"\n    },\n    \"created_time\": {\n      \"type\": \"string\",\n\
  \      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the survey was created.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL path to the survey resource in the API.\"\n    },\n    \"responses_url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL path to retrieve the survey responses.\"\n    },\n    \"sentiment_analysis_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether sentiment analysis is enabled for this survey.\"\n    },\n    \"questions\": {\n      \"type\": \"array\",\n      \"description\": \"The list of questions in the survey.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SurveyQuestion\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"SurveyQuestion\": {\n      \"type\": \"object\",\n      \"description\": \"A question within a Hotjar survey.\",\n      \"required\": [\"id\", \"text\", \"type\"],\n      \"properties\": {\n        \"id\": {\n          \"type\"\
  : \"integer\",\n          \"description\": \"The unique identifier for the question.\"\n        },\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"The text content of the question displayed to respondents.\",\n          \"minLength\": 1\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of question.\",\n          \"enum\": [\"long-text\", \"short-text\", \"rating\", \"multiple-choice\", \"nps\", \"single-choice\"]\n        },\n        \"is_required\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the question requires an answer before submission.\"\n        },\n        \"choices\": {\n          \"type\": [\"array\", \"null\"],\n          \"description\": \"The list of answer choices for multiple-choice questions. Null for open-ended question types.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"labels\": {\n          \"\
  type\": [\"object\", \"null\"],\n          \"description\": \"Labels for rating or scale questions. Null for other question types.\"\n        },\n        \"image_url\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"URL of an image attached to the question. Null if no image is attached.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hotjar/refs/heads/main/json-schema/hotjar-survey-schema.json
tags: []
title: Hotjar Survey
---
