---
description: A Retool application built in the visual editor, connecting to databases and APIs.
layout: schema
name: Retool App
properties_list:
- description: The unique identifier for the app.
  name: id
  type: string
- description: The name of the application.
  name: name
  type: string
- description: A description of the application's purpose.
  name: description
  type: string
- description: The identifier of the folder containing this app.
  name: folderId
  type: string
- description: The email of the user who created the app.
  name: createdBy
  type: string
- description: Resource identifiers used by this app.
  name: resources
  type: array
- description: Timestamp when the app was created.
  name: createdAt
  type: string
- description: Timestamp when the app was last updated.
  name: updatedAt
  type: string
provider_name: Retool
provider_slug: retool
schema_file: json-schema/retool-app-schema.json
slug: retool-app
source_filename: retool-app-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/retool/json-schema/retool-app-schema.json\",\n  \"title\": \"Retool App\",\n  \"description\": \"A Retool application built in the visual editor, connecting to databases and APIs.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the app.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the application's purpose.\"\n    },\n    \"folderId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the folder containing this app.\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"The email of the user who created\
  \ the app.\"\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"description\": \"Resource identifiers used by this app.\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the app was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the app was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/retool/refs/heads/main/json-schema/retool-app-schema.json
tags:
- Admin Panel
- Dashboard
- Internal Tools
- Low Code
- No Code
title: Retool App
---
