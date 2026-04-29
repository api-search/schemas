---
description: The crop properties of an image.
layout: schema
name: CropProperties
properties_list:
- description: The offset from the left edge, as a fraction of the image width.
  name: offsetLeft
  type: number
- description: The offset from the right edge, as a fraction of the image width.
  name: offsetRight
  type: number
- description: The offset from the top edge, as a fraction of the image height.
  name: offsetTop
  type: number
- description: The offset from the bottom edge, as a fraction of the image height.
  name: offsetBottom
  type: number
- description: The clockwise rotation angle of the crop rectangle.
  name: angle
  type: number
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-crop-properties-schema.json
slug: google-docs-v1-crop-properties
source_filename: google-docs-v1-crop-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CropProperties\",\n  \"type\": \"object\",\n  \"description\": \"The crop properties of an image.\",\n  \"properties\": {\n    \"offsetLeft\": {\n      \"type\": \"number\",\n      \"description\": \"The offset from the left edge, as a fraction of the image width.\"\n    },\n    \"offsetRight\": {\n      \"type\": \"number\",\n      \"description\": \"The offset from the right edge, as a fraction of the image width.\"\n    },\n    \"offsetTop\": {\n      \"type\": \"number\",\n      \"description\": \"The offset from the top edge, as a fraction of the image height.\"\n    },\n    \"offsetBottom\": {\n      \"type\": \"number\",\n      \"description\": \"The offset from the bottom edge, as a fraction of the image height.\"\n    },\n    \"angle\": {\n      \"type\": \"number\",\n      \"description\": \"The clockwise rotation angle of the crop rectangle.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-crop-properties-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: CropProperties
---
