---
description: Successful response containing rendered image URLs.
layout: schema
name: GetImagesResponseBody
properties_list:
- description: For successful requests, this value is always `null`.
  name: err
  type: 'null'
- description: A map from node IDs to URLs of the rendered images.
  name: images
  type: object
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-images-get-images-response-body-schema.json
slug: figma-images-get-images-response-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetImagesResponseBody\",\n  \"type\": \"object\",\n  \"description\": \"Successful response containing rendered image URLs.\",\n  \"properties\": {\n    \"err\": {\n      \"type\": \"null\",\n      \"description\": \"For successful requests, this value is always `null`.\"\n    },\n    \"images\": {\n      \"type\": \"object\",\n      \"description\": \"A map from node IDs to URLs of the rendered images.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-images-get-images-response-body-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: GetImagesResponseBody
---
