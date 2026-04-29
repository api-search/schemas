---
description: A response indicating an error occurred.
layout: schema
name: ErrorResponsePayload
properties_list:
- description: For erroneous requests, this value is always `true`.
  name: error
  type: boolean
- description: Status code
  name: status
  type: number
- description: A string describing the error
  name: message
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-payments-error-response-payload-schema.json
slug: figma-payments-error-response-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponsePayload\",\n  \"type\": \"object\",\n  \"description\": \"A response indicating an error occurred.\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"boolean\",\n      \"description\": \"For erroneous requests, this value is always `true`.\"\n    },\n    \"status\": {\n      \"type\": \"number\",\n      \"description\": \"Status code\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A string describing the error\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-payments-error-response-payload-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: ErrorResponsePayload
---
