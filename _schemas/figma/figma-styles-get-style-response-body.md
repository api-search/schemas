---
description: Successful response containing style metadata.
layout: schema
name: GetStyleResponseBody
properties_list:
- description: The status of the request.
  name: status
  type: number
- description: For successful requests, this value is always `false`.
  name: error
  type: boolean
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-styles-get-style-response-body-schema.json
slug: figma-styles-get-style-response-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetStyleResponseBody\",\n  \"type\": \"object\",\n  \"description\": \"Successful response containing style metadata.\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"number\",\n      \"description\": \"The status of the request.\"\n    },\n    \"error\": {\n      \"type\": \"boolean\",\n      \"description\": \"For successful requests, this value is always `false`.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-styles-get-style-response-body-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: GetStyleResponseBody
---
