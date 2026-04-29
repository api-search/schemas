---
description: A comment attached to an Airtable record. Comments support user mentions using the @[usrXXXXXXXX] syntax and are used for collaboration and discussion within records.
layout: schema
name: Airtable Comment
properties_list:
- description: The unique identifier for the comment.
  name: id
  type: string
- description: The text content of the comment. May include user mentions in the format @[usrXXXXXXXX].
  name: text
  type: string
- description: The user who created the comment.
  name: author
  type: object
- description: The time when the comment was created in ISO 8601 format.
  name: createdTime
  type: string
- description: The time when the comment was last updated. Null if the comment has not been edited.
  name: lastUpdatedTime
  type:
  - string
  - 'null'
provider_name: Airtable
provider_slug: airtable
schema_file: json-schema/airtable-comment-schema.json
slug: airtable-comment
source_filename: airtable-comment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.airtable.com/comment.json\",\n  \"title\": \"Airtable Comment\",\n  \"description\": \"A comment attached to an Airtable record. Comments support user mentions using the @[usrXXXXXXXX] syntax and are used for collaboration and discussion within records.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the comment.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The text content of the comment. May include user mentions in the format @[usrXXXXXXXX].\"\n    },\n    \"author\": {\n      \"type\": \"object\",\n      \"description\": \"The user who created the comment.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the comment author (starts with 'usr').\"\n        },\n\
  \        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address of the comment author.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the comment author.\"\n        }\n      },\n      \"required\": [\"id\", \"email\", \"name\"]\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the comment was created in ISO 8601 format.\"\n    },\n    \"lastUpdatedTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The time when the comment was last updated. Null if the comment has not been edited.\"\n    }\n  },\n  \"required\": [\"id\", \"text\", \"createdTime\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/json-schema/airtable-comment-schema.json
tags:
- Applications
- Collaboration
- Data
- Databases
- Low-Code
- Productivity
- Spreadsheets
title: Airtable Comment
---
