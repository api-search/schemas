---
description: A description of a user.
layout: schema
name: User
properties_list:
- description: Unique stable id of the user.
  name: id
  type: string
- description: Name of the user.
  name: handle
  type: string
- description: URL link to the user's profile image.
  name: imgUrl
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-component-sets-user-schema.json
slug: figma-component-sets-user
source_filename: figma-component-sets-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"description\": \"A description of a user.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique stable id of the user.\"\n    },\n    \"handle\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the user.\"\n    },\n    \"imgUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL link to the user's profile image.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-component-sets-user-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: User
---
