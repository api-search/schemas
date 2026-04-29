---
description: A file within a Figma project.
layout: schema
name: ProjectFile
properties_list:
- description: The file key.
  name: key
  type: string
- description: The name of the file.
  name: name
  type: string
- description: A URL to a thumbnail image of the file.
  name: thumbnail_url
  type: string
- description: The UTC ISO 8601 time at which the file was last modified.
  name: last_modified
  type: string
- description: Branches of this file, if branch_data was requested.
  name: branches
  type: array
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-project-file-schema.json
slug: figma-rest-project-file
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProjectFile\",\n  \"type\": \"object\",\n  \"description\": \"A file within a Figma project.\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The file key.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the file.\"\n    },\n    \"thumbnail_url\": {\n      \"type\": \"string\",\n      \"description\": \"A URL to a thumbnail image of the file.\"\n    },\n    \"last_modified\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 time at which the file was last modified.\"\n    },\n    \"branches\": {\n      \"type\": \"array\",\n      \"description\": \"Branches of this file, if branch_data was requested.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-project-file-schema.json
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
