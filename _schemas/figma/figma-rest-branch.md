---
description: Information about a branch of a Figma file.
layout: schema
name: Branch
properties_list:
- description: The key of the branch file.
  name: key
  type: string
- description: The name of the branch.
  name: name
  type: string
- description: A URL to a thumbnail image of the branch.
  name: thumbnail_url
  type: string
- description: The UTC ISO 8601 time at which the branch was last modified.
  name: last_modified
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-branch-schema.json
slug: figma-rest-branch
source_filename: figma-rest-branch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Branch\",\n  \"type\": \"object\",\n  \"description\": \"Information about a branch of a Figma file.\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the branch file.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the branch.\"\n    },\n    \"thumbnail_url\": {\n      \"type\": \"string\",\n      \"description\": \"A URL to a thumbnail image of the branch.\"\n    },\n    \"last_modified\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 time at which the branch was last modified.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-branch-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: Branch
---
