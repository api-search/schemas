---
description: An application registered in a DreamFactory instance, associated with an API key and optional default role for access control.
layout: schema
name: DreamFactory App
properties_list:
- description: Unique identifier for the application.
  name: id
  type: integer
- description: Name of the application.
  name: name
  type: string
- description: API key assigned to the application.
  name: api_key
  type: string
- description: Description of the application.
  name: description
  type: string
- description: Whether the application is active.
  name: is_active
  type: boolean
- description: Application type identifier.
  name: type
  type: integer
- description: Default role ID assigned to the application.
  name: role_id
  type: integer
- description: Timestamp when the application was created.
  name: created_date
  type: string
- description: Timestamp when the application was last modified.
  name: last_modified_date
  type: string
provider_name: DreamFactory
provider_slug: dreamfactory
schema_file: json-schema/dreamfactory-app.json
slug: dreamfactory-app
source_filename: dreamfactory-app.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/json-schema/dreamfactory-app.json\",\n  \"title\": \"DreamFactory App\",\n  \"description\": \"An application registered in a DreamFactory instance, associated with an API key and optional default role for access control.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the application.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the application.\"\n    },\n    \"api_key\": {\n      \"type\": \"string\",\n      \"description\": \"API key assigned to the application.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the application.\"\n    },\n    \"is_active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the\
  \ application is active.\"\n    },\n    \"type\": {\n      \"type\": \"integer\",\n      \"description\": \"Application type identifier.\"\n    },\n    \"role_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Default role ID assigned to the application.\"\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the application was created.\"\n    },\n    \"last_modified_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the application was last modified.\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/json-schema/dreamfactory-app.json
tags:
- Automation
- Deployment
- Documentation
- Generation
- Security
title: DreamFactory App
---
