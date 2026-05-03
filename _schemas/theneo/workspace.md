---
description: A Workspace is an organizational unit on the Theneo platform that groups related API documentation projects together.
layout: schema
name: Theneo Workspace
properties_list:
- description: The unique identifier of the workspace.
  name: id
  type: string
- description: The name of the workspace.
  name: name
  type: string
- description: The URL-friendly slug of the workspace.
  name: slug
  type: string
provider_name: Theneo
provider_slug: theneo
schema_file: json-schema/workspace.json
slug: workspace
source_filename: workspace.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/theneo/blob/main/json-schema/workspace.json\",\n  \"title\": \"Theneo Workspace\",\n  \"description\": \"A Workspace is an organizational unit on the Theneo platform that groups related API documentation projects together.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the workspace.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workspace.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The URL-friendly slug of the workspace.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/theneo/refs/heads/main/json-schema/workspace.json
tags:
- Change Logs
- Documentation
- Platform
title: Theneo Workspace
---
