---
description: Schema for a Redux action object. Actions are plain JavaScript objects that represent an intention to change the state. Every action must have a type field.
layout: schema
name: Redux Action
properties_list:
- description: A string constant identifying the kind of action being performed. By convention written in SCREAMING_SNAKE_CASE.
  name: type
  type: string
- description: Any data that accompanies the action. Follows the Flux Standard Action convention.
  name: payload
  type: object
- description: When true, the payload is treated as an error object. Follows the Flux Standard Action convention.
  name: error
  type: boolean
- description: Extra information that is not part of the payload. Follows the Flux Standard Action convention.
  name: meta
  type: object
provider_name: Redux
provider_slug: redux
schema_file: json-schema/redux-action-schema.json
slug: redux-action
source_filename: redux-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/redux/json-schema/redux-action-schema.json\",\n  \"title\": \"Redux Action\",\n  \"description\": \"Schema for a Redux action object. Actions are plain JavaScript objects that represent an intention to change the state. Every action must have a type field.\",\n  \"type\": \"object\",\n  \"required\": [\"type\"],\n  \"properties\": {\n    \"type\": {\n      \"description\": \"A string constant identifying the kind of action being performed. By convention written in SCREAMING_SNAKE_CASE.\",\n      \"type\": \"string\",\n      \"examples\": [\n        \"INCREMENT\",\n        \"USER_FETCH_SUCCEEDED\",\n        \"todos/addTodo\",\n        \"counter/increment\"\n      ]\n    },\n    \"payload\": {\n      \"description\": \"Any data that accompanies the action. Follows the Flux Standard Action convention.\",\n      \"oneOf\": [\n        {\"type\": \"string\"},\n        {\"\
  type\": \"number\"},\n        {\"type\": \"boolean\"},\n        {\"type\": \"object\"},\n        {\"type\": \"array\"},\n        {\"type\": \"null\"}\n      ]\n    },\n    \"error\": {\n      \"description\": \"When true, the payload is treated as an error object. Follows the Flux Standard Action convention.\",\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"meta\": {\n      \"description\": \"Extra information that is not part of the payload. Follows the Flux Standard Action convention.\",\n      \"type\": \"object\",\n      \"additionalProperties\": true\n    }\n  },\n  \"additionalProperties\": false,\n  \"examples\": [\n    {\n      \"type\": \"INCREMENT\"\n    },\n    {\n      \"type\": \"todos/addTodo\",\n      \"payload\": {\n        \"id\": 1,\n        \"text\": \"Buy milk\",\n        \"completed\": false\n      }\n    },\n    {\n      \"type\": \"USER_FETCH_FAILED\",\n      \"payload\": {\n        \"message\": \"Network request failed\"\n      },\n     \
  \ \"error\": true\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/redux/refs/heads/main/json-schema/redux-action-schema.json
tags:
- Flux Architecture
- Frontend
- Javascript
- Predictable State
- React
- State Management
- Typescript
title: Redux Action
---
