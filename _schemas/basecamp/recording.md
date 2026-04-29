---
description: A generic recording object representing any Basecamp content resource such as a message, to-do, document, comment, or upload.
layout: schema
name: Recording
properties_list:
- description: Recording ID
  name: id
  type: integer
- description: Recording status
  name: status
  type: string
- description: Whether this recording is visible to client users
  name: visible_to_clients
  type: boolean
- description: Timestamp when the recording was created
  name: created_at
  type: string
- description: Timestamp when the recording was last updated
  name: updated_at
  type: string
- description: Title or summary of the recording
  name: title
  type: string
- description: Whether this recording inherits its status from a parent
  name: inherits_status
  type: boolean
- description: Recording type (e.g., Message, Todo, Document)
  name: type
  type: string
- description: API URL for this recording
  name: url
  type: string
- description: Web URL for this recording
  name: app_url
  type: string
- description: ''
  name: bucket
  type: object
- description: ''
  name: creator
  type: object
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/recording-schema.json
slug: recording
source_filename: recording-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/recording-schema.json\",\n  \"title\": \"Recording\",\n  \"type\": \"object\",\n  \"description\": \"A generic recording object representing any Basecamp content resource such as a message, to-do, document, comment, or upload.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Recording ID\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Recording status\",\n      \"enum\": [\n        \"active\",\n        \"archived\",\n        \"trashed\"\n      ]\n    },\n    \"visible_to_clients\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this recording is visible to client users\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the recording was created\"\n    },\n\
  \    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the recording was last updated\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title or summary of the recording\"\n    },\n    \"inherits_status\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this recording inherits its status from a parent\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Recording type (e.g., Message, Todo, Document)\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL for this recording\"\n    },\n    \"app_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Web URL for this recording\"\n    },\n    \"bucket\": {\n      \"$ref\": \"#/components/schemas/BucketRef\"\n    },\n    \"creator\": {\n      \"$ref\": \"#/components/schemas/PersonRef\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/recording-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Recording
---
