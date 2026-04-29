---
description: An emoji reaction left on a comment.
layout: schema
name: Reaction
properties_list:
- description: The emoji used for the reaction.
  name: emoji
  type: string
- description: The UTC ISO 8601 time at which the reaction was left.
  name: created_at
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-reaction-schema.json
slug: figma-rest-reaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Reaction\",\n  \"type\": \"object\",\n  \"description\": \"An emoji reaction left on a comment.\",\n  \"properties\": {\n    \"emoji\": {\n      \"type\": \"string\",\n      \"description\": \"The emoji used for the reaction.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 time at which the reaction was left.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-reaction-schema.json
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
