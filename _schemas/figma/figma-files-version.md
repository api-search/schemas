---
description: A version of a file.
layout: schema
name: Version
properties_list:
- description: Unique identifier for version.
  name: id
  type: string
- description: The UTC ISO 8601 time at which the version was created.
  name: createdAt
  type: string
- description: The label given to the version in the editor.
  name: label
  type: '[''string'', ''null'']'
- description: The description of the version as entered in the editor.
  name: description
  type: '[''string'', ''null'']'
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-files-version-schema.json
slug: figma-files-version
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Version\",\n  \"type\": \"object\",\n  \"description\": \"A version of a file.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for version.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 time at which the version was created.\"\n    },\n    \"label\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The label given to the version in the editor.\"\n    },\n    \"description\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The description of the version as entered in the editor.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-files-version-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: Version
---
