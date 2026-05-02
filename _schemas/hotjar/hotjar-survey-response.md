---
description: A single response to a Hotjar survey, containing the answers provided by a respondent along with optional comments and tags.
layout: schema
name: Hotjar Survey Response
properties_list:
- description: The unique identifier for the survey response.
  name: id
  type: string
- description: The list of answers provided by the respondent.
  name: answers
  type: array
- description: An optional comment provided by the respondent.
  name: comment
  type:
  - string
  - 'null'
- description: Tags associated with this survey response for categorization.
  name: tags
  type: array
provider_name: hotjar
provider_slug: hotjar
schema_file: json-schema/hotjar-survey-response-schema.json
slug: hotjar-survey-response
source_filename: hotjar-survey-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://hotjar.com/schemas/hotjar/survey-response.json\",\n  \"title\": \"Hotjar Survey Response\",\n  \"description\": \"A single response to a Hotjar survey, containing the answers provided by a respondent along with optional comments and tags.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"answers\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the survey response.\"\n    },\n    \"answers\": {\n      \"type\": \"array\",\n      \"description\": \"The list of answers provided by the respondent.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SurveyAnswer\"\n      }\n    },\n    \"comment\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An optional comment provided by the respondent.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with\
  \ this survey response for categorization.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SurveyResponseTag\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"SurveyAnswer\": {\n      \"type\": \"object\",\n      \"description\": \"An individual answer to a survey question.\",\n      \"required\": [\"question_id\", \"answer\"],\n      \"properties\": {\n        \"question_id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the question being answered.\"\n        },\n        \"answer\": {\n          \"type\": \"string\",\n          \"description\": \"The text of the answer provided by the respondent.\"\n        }\n      }\n    },\n    \"SurveyResponseTag\": {\n      \"type\": \"object\",\n      \"description\": \"A tag associated with a survey response.\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the tag.\"\n        }\n      }\n  \
  \  }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hotjar/refs/heads/main/json-schema/hotjar-survey-response-schema.json
tags: []
title: Hotjar Survey Response
---
