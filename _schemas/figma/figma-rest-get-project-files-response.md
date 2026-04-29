---
description: Response from the Get Project Files endpoint.
layout: schema
name: GetProjectFilesResponse
properties_list:
- description: The name of the project.
  name: name
  type: string
- description: ''
  name: files
  type: array
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-get-project-files-response-schema.json
slug: figma-rest-get-project-files-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetProjectFilesResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response from the Get Project Files endpoint.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the project.\"\n    },\n    \"files\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-get-project-files-response-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: GetProjectFilesResponse
---
