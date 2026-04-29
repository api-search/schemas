---
description: An Amazon Lex intent representing an action a user can perform.
layout: schema
name: Intent
properties_list:
- description: The unique identifier assigned to the intent.
  name: intentId
  type: string
- description: The name of the intent.
  name: intentName
  type: string
- description: The description of the intent.
  name: description
  type: string
- description: The identifier of the bot associated with this intent.
  name: botId
  type: string
- description: The version of the bot associated with this intent.
  name: botVersion
  type: string
- description: The language and locale of the intent.
  name: localeId
  type: string
- description: A timestamp of the date and time the intent was created.
  name: creationDateTime
  type: string
provider_name: Amazon Lex
provider_slug: amazon-lex
schema_file: json-schema/amazon-lex-intent-schema.json
slug: amazon-lex-intent
source_filename: amazon-lex-intent-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/json-schema/amazon-lex-intent-schema.json\",\n  \"title\": \"Intent\",\n  \"description\": \"An Amazon Lex intent representing an action a user can perform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"intentId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier assigned to the intent.\",\n      \"example\": \"ABCDEF123456\"\n    },\n    \"intentName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the intent.\",\n      \"example\": \"OrderPizza\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the intent.\"\n    },\n    \"botId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the bot associated with this intent.\"\n    },\n    \"botVersion\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The version of the bot associated with this intent.\"\n    },\n    \"localeId\": {\n      \"type\": \"string\",\n      \"description\": \"The language and locale of the intent.\",\n      \"example\": \"en_US\"\n    },\n    \"creationDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"A timestamp of the date and time the intent was created.\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/json-schema/amazon-lex-intent-schema.json
tags: []
title: Intent
---
