---
description: An Amazon Lex V2 bot for building conversational interfaces.
layout: schema
name: Bot
properties_list:
- description: The unique identifier assigned to the bot.
  name: botId
  type: string
- description: The name specified for the bot.
  name: botName
  type: string
- description: The current status of the bot.
  name: botStatus
  type: string
- description: The description of the bot.
  name: description
  type: string
- description: The Amazon Resource Name (ARN) of the role assumed by the bot.
  name: roleArn
  type: string
- description: A timestamp of the date and time the bot was created.
  name: creationDateTime
  type: string
- description: A timestamp of the date and time the bot was last updated.
  name: lastUpdatedDateTime
  type: string
provider_name: Amazon Lex
provider_slug: amazon-lex
schema_file: json-schema/amazon-lex-bot-schema.json
slug: amazon-lex-bot
source_filename: amazon-lex-bot-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/json-schema/amazon-lex-bot-schema.json\",\n  \"title\": \"Bot\",\n  \"description\": \"An Amazon Lex V2 bot for building conversational interfaces.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"botId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier assigned to the bot.\",\n      \"example\": \"ABCDEF123456\"\n    },\n    \"botName\": {\n      \"type\": \"string\",\n      \"description\": \"The name specified for the bot.\",\n      \"example\": \"CustomerServiceBot\"\n    },\n    \"botStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the bot.\",\n      \"example\": \"Available\",\n      \"enum\": [\n        \"Creating\",\n        \"Available\",\n        \"Inactive\",\n        \"Deleting\",\n        \"Failed\",\n        \"Versioning\",\n  \
  \      \"Importing\",\n        \"Updating\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the bot.\"\n    },\n    \"roleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the role assumed by the bot.\"\n    },\n    \"creationDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"A timestamp of the date and time the bot was created.\",\n      \"format\": \"date-time\"\n    },\n    \"lastUpdatedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"A timestamp of the date and time the bot was last updated.\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lex/refs/heads/main/json-schema/amazon-lex-bot-schema.json
tags: []
title: Bot
---
