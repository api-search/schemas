---
description: ''
layout: schema
name: PutDevResourcesResponseBody
properties_list:
- description: An array of links updated.
  name: linksUpdated
  type: array
- description: An array of errors.
  name: errors
  type: array
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-dev-resources-put-dev-resources-response-body-schema.json
slug: figma-dev-resources-put-dev-resources-response-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PutDevResourcesResponseBody\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"linksUpdated\": {\n      \"type\": \"array\",\n      \"description\": \"An array of links updated.\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"An array of errors.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-dev-resources-put-dev-resources-response-body-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: PutDevResourcesResponseBody
---
