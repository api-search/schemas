---
description: Response from the Get Images endpoint.
layout: schema
name: GetImagesResponse
properties_list:
- description: If present, indicates an error rendering the images.
  name: err
  type: '[''string'', ''null'']'
- description: A mapping from node IDs to URLs of the rendered images. Image URLs expire after 14 days.
  name: images
  type: object
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-get-images-response-schema.json
slug: figma-rest-get-images-response
source_filename: figma-rest-get-images-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetImagesResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response from the Get Images endpoint.\",\n  \"properties\": {\n    \"err\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"If present, indicates an error rendering the images.\"\n    },\n    \"images\": {\n      \"type\": \"object\",\n      \"description\": \"A mapping from node IDs to URLs of the rendered images. Image URLs expire after 14 days.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-get-images-response-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: GetImagesResponse
---
