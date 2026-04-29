---
description: Successful response containing project files.
layout: schema
name: GetProjectFilesResponseBody
properties_list:
- description: The project's name.
  name: name
  type: string
- description: An array of files.
  name: files
  type: array
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-projects-get-project-files-response-body-schema.json
slug: figma-projects-get-project-files-response-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetProjectFilesResponseBody\",\n  \"type\": \"object\",\n  \"description\": \"Successful response containing project files.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The project's name.\"\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"description\": \"An array of files.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-projects-get-project-files-response-body-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: GetProjectFilesResponseBody
---
