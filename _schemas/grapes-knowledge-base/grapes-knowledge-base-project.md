---
description: A project resource within the Grapes knowledge management platform.
layout: schema
name: Grapes Project
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: modifiedAt
  type: string
- description: HATEOAS links to related resources.
  name: _links
  type: object
provider_name: Grapes Knowledge Base
provider_slug: grapes-knowledge-base
schema_file: json-schema/grapes-knowledge-base-project-schema.json
slug: grapes-knowledge-base-project
source_filename: grapes-knowledge-base-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/grapes-knowledge-base/refs/heads/main/json-schema/grapes-knowledge-base-project-schema.json\",\n  \"title\": \"Grapes Project\",\n  \"description\": \"A project resource within the Grapes knowledge management platform.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": { \"type\": \"string\" },\n    \"name\": { \"type\": \"string\" },\n    \"description\": { \"type\": \"string\" },\n    \"createdAt\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"modifiedAt\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"_links\": {\n      \"type\": \"object\",\n      \"description\": \"HATEOAS links to related resources.\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"href\": { \"type\": \"string\", \"format\": \"uri\" }\n  \
  \      }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/grapes-knowledge-base/refs/heads/main/json-schema/grapes-knowledge-base-project-schema.json
tags:
- Knowledge Management
- Knowledge Base
- Data Management
- Automation
- HATEOAS
title: Grapes Project
---
