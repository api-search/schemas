---
description: Represents a label applied to Confluence content.
layout: schema
name: Label
properties_list:
- description: The unique identifier of the label.
  name: id
  type: string
- description: The name of the label.
  name: name
  type: string
- description: The prefix of the label (global, my, team).
  name: prefix
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-label-schema.json
slug: confluence-cloud-v2-label
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Label\",\n  \"type\": \"object\",\n  \"description\": \"Represents a label applied to Confluence content.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the label.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the label.\"\n    },\n    \"prefix\": {\n      \"type\": \"string\",\n      \"description\": \"The prefix of the label (global, my, team).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-label-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: Label
---
