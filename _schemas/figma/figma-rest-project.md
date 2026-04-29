---
description: A Figma project within a team.
layout: schema
name: Project
properties_list:
- description: The ID of the project.
  name: id
  type: string
- description: The name of the project.
  name: name
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-project-schema.json
slug: figma-rest-project
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Project\",\n  \"type\": \"object\",\n  \"description\": \"A Figma project within a team.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the project.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the project.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-project-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: Project
---
