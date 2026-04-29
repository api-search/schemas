---
description: A reaction left by a user.
layout: schema
name: Reaction
properties_list:
- description: The emoji used for the reaction.
  name: emoji
  type: string
- description: The UTC ISO 8601 time at which the reaction was left.
  name: createdAt
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-files-reaction-schema.json
slug: figma-files-reaction
source_filename: figma-files-reaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Reaction\",\n  \"type\": \"object\",\n  \"description\": \"A reaction left by a user.\",\n  \"properties\": {\n    \"emoji\": {\n      \"type\": \"string\",\n      \"description\": \"The emoji used for the reaction.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 time at which the reaction was left.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-files-reaction-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: Reaction
---
