---
description: RemoveBackgroundRequest from Adobe Photoshop API
layout: schema
name: RemoveBackgroundRequest
properties_list:
- description: ''
  name: image
  type: object
- description: cutout removes the background, mask returns a grayscale mask.
  name: mode
  type: string
- description: ''
  name: output
  type: object
- description: Whether to trim whitespace around the subject.
  name: trim
  type: boolean
- description: Optional replacement background color.
  name: backgroundColor
  type: object
- description: Level of color decontamination to apply.
  name: colorDecontamination
  type: integer
provider_name: Adobe Photoshop
provider_slug: adobe-photoshop
schema_file: json-schema/adobe-photoshop-api-remove-background-request-schema.json
slug: adobe-photoshop-api-remove-background-request
source_filename: adobe-photoshop-api-remove-background-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-remove-background-request-schema.json\",\n  \"title\": \"RemoveBackgroundRequest\",\n  \"description\": \"RemoveBackgroundRequest from Adobe Photoshop API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"image\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"source\"\n      ],\n      \"properties\": {\n        \"source\": {\n          \"type\": \"object\",\n          \"required\": [\n            \"url\"\n          ],\n          \"properties\": {\n            \"url\": {\n              \"type\": \"string\",\n              \"description\": \"Pre-signed GET URL of the source image.\"\n            }\n          }\n        }\n      }\n    },\n    \"mode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"cutout\",\n        \"mask\"\n      ],\n      \"\
  default\": \"cutout\",\n      \"description\": \"cutout removes the background, mask returns a grayscale mask.\",\n      \"example\": \"cutout\"\n    },\n    \"output\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"mediaType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"image/jpeg\",\n            \"image/png\"\n          ],\n          \"description\": \"Output format.\"\n        }\n      }\n    },\n    \"trim\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether to trim whitespace around the subject.\",\n      \"example\": true\n    },\n    \"backgroundColor\": {\n      \"type\": \"object\",\n      \"description\": \"Optional replacement background color.\",\n      \"properties\": {\n        \"red\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"maximum\": 255\n        },\n        \"green\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n        \
  \  \"maximum\": 255\n        },\n        \"blue\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"maximum\": 255\n        },\n        \"alpha\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 1\n        }\n      }\n    },\n    \"colorDecontamination\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Level of color decontamination to apply.\",\n      \"example\": 1920\n    }\n  },\n  \"required\": [\n    \"image\",\n    \"output\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-remove-background-request-schema.json
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
title: RemoveBackgroundRequest
---
