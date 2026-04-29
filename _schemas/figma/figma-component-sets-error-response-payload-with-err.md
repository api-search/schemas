---
description: A response indicating an error occurred.
layout: schema
name: ErrorResponsePayloadWithErr
properties_list:
- description: Status code
  name: status
  type: number
- description: A string describing the error
  name: err
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-component-sets-error-response-payload-with-err-schema.json
slug: figma-component-sets-error-response-payload-with-err
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponsePayloadWithErr\",\n  \"type\": \"object\",\n  \"description\": \"A response indicating an error occurred.\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"number\",\n      \"description\": \"Status code\"\n    },\n    \"err\": {\n      \"type\": \"string\",\n      \"description\": \"A string describing the error\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-component-sets-error-response-payload-with-err-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: ErrorResponsePayloadWithErr
---
