---
description: Response from the Get File Components endpoint.
layout: schema
name: GetFileComponentsResponse
properties_list:
- description: ''
  name: error
  type: boolean
- description: ''
  name: status
  type: integer
- description: ''
  name: meta
  type: object
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-get-file-components-response-schema.json
slug: figma-rest-get-file-components-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetFileComponentsResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response from the Get File Components endpoint.\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"boolean\"\n    },\n    \"status\": {\n      \"type\": \"integer\"\n    },\n    \"meta\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-get-file-components-response-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: GetFileComponentsResponse
---
