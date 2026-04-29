---
description: The properties of an image.
layout: schema
name: ImageProperties
properties_list:
- description: A URI to the image with a default lifetime of 30 minutes.
  name: contentUri
  type: string
- description: The source URI of the image.
  name: sourceUri
  type: string
- description: The brightness effect of the image, from -1.0 to 1.0.
  name: brightness
  type: number
- description: The contrast effect of the image, from -1.0 to 1.0.
  name: contrast
  type: number
- description: The transparency effect of the image, from 0.0 to 1.0.
  name: transparency
  type: number
- description: The clockwise rotation angle of the image, in radians.
  name: angle
  type: number
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-image-properties-schema.json
slug: google-docs-v1-image-properties
source_filename: google-docs-v1-image-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImageProperties\",\n  \"type\": \"object\",\n  \"description\": \"The properties of an image.\",\n  \"properties\": {\n    \"contentUri\": {\n      \"type\": \"string\",\n      \"description\": \"A URI to the image with a default lifetime of 30 minutes.\"\n    },\n    \"sourceUri\": {\n      \"type\": \"string\",\n      \"description\": \"The source URI of the image.\"\n    },\n    \"brightness\": {\n      \"type\": \"number\",\n      \"description\": \"The brightness effect of the image, from -1.0 to 1.0.\"\n    },\n    \"contrast\": {\n      \"type\": \"number\",\n      \"description\": \"The contrast effect of the image, from -1.0 to 1.0.\"\n    },\n    \"transparency\": {\n      \"type\": \"number\",\n      \"description\": \"The transparency effect of the image, from 0.0 to 1.0.\"\n    },\n    \"angle\": {\n      \"type\": \"number\",\n      \"description\": \"The clockwise rotation angle\
  \ of the image, in radians.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-image-properties-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: ImageProperties
---
