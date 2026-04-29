---
description: A file within a project.
layout: schema
name: ProjectFile
properties_list:
- description: The file's key.
  name: key
  type: string
- description: The file's name.
  name: name
  type: string
- description: The file's thumbnail URL.
  name: thumbnail_url
  type: string
- description: The UTC ISO 8601 time at which the file was last modified.
  name: last_modified
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-projects-project-file-schema.json
slug: figma-projects-project-file
source_filename: figma-projects-project-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProjectFile\",\n  \"type\": \"object\",\n  \"description\": \"A file within a project.\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The file's key.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The file's name.\"\n    },\n    \"thumbnail_url\": {\n      \"type\": \"string\",\n      \"description\": \"The file's thumbnail URL.\"\n    },\n    \"last_modified\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 time at which the file was last modified.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-projects-project-file-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: ProjectFile
---
