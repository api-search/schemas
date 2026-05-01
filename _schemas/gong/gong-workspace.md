---
description: Represents a workspace in the Gong platform, used to organize and segment data within the organization.
layout: schema
name: Gong Workspace
properties_list:
- description: Unique identifier for the workspace.
  name: id
  type: string
- description: Name of the workspace.
  name: name
  type: string
- description: Description of the workspace.
  name: description
  type: string
provider_name: Gong
provider_slug: gong
schema_file: json-schema/gong-workspace-schema.json
slug: gong-workspace
source_filename: gong-workspace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gong/blob/main/json-schema/gong-workspace-schema.json\",\n  \"title\": \"Gong Workspace\",\n  \"description\": \"Represents a workspace in the Gong platform, used to organize and segment data within the organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the workspace.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workspace.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the workspace.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/json-schema/gong-workspace-schema.json
tags: []
title: Gong Workspace
---
