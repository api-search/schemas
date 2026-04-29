---
description: Response body for successful dev resource deletion.
layout: schema
name: DeleteDevResourceResponseBody
properties_list:
- description: The status of the request.
  name: status
  type: number
- description: For successful requests, this value is always `false`.
  name: error
  type: boolean
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-files-delete-dev-resource-response-body-schema.json
slug: figma-files-delete-dev-resource-response-body
source_filename: figma-files-delete-dev-resource-response-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteDevResourceResponseBody\",\n  \"type\": \"object\",\n  \"description\": \"Response body for successful dev resource deletion.\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"number\",\n      \"description\": \"The status of the request.\"\n    },\n    \"error\": {\n      \"type\": \"boolean\",\n      \"description\": \"For successful requests, this value is always `false`.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-files-delete-dev-resource-response-body-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: DeleteDevResourceResponseBody
---
