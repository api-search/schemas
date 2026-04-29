---
description: A Figma user account.
layout: schema
name: User
properties_list:
- description: Unique stable ID of the user.
  name: id
  type: string
- description: Display name of the user.
  name: handle
  type: string
- description: URL of the user's profile image.
  name: img_url
  type: string
- description: Email address associated with the user's account.
  name: email
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-user-schema.json
slug: figma-rest-user
source_filename: figma-rest-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"description\": \"A Figma user account.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique stable ID of the user.\"\n    },\n    \"handle\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the user.\"\n    },\n    \"img_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the user's profile image.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email address associated with the user's account.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-user-schema.json
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
