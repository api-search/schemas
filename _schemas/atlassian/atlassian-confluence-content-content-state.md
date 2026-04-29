---
description: ''
layout: schema
name: ContentState
properties_list:
- description: identifier of content state. If 0, 1, or 2, this is a default space state
  name: id
  type: integer
- description: name of content state.
  name: name
  type: string
- description: hex string representing color of state
  name: color
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-content-state-schema.json
slug: atlassian-confluence-content-content-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentState\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"identifier of content state. If 0, 1, or 2, this is a default space state\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"name of content state.\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"hex string representing color of state\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-content-state-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ContentState
---
