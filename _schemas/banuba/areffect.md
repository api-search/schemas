---
description: A Banuba augmented reality effect that can be applied to a face in a video frame.
layout: schema
name: AREffect
properties_list:
- description: Unique identifier for the AR effect.
  name: effectId
  type: string
- description: Human-readable name of the effect.
  name: name
  type: string
- description: Category of the effect.
  name: category
  type: string
- description: URL of a preview image for the effect.
  name: previewUrl
  type: string
- description: URL of the effect bundle file.
  name: effectUrl
  type: string
- description: Platforms supported by this effect.
  name: platforms
  type: array
- description: Tags describing the effect.
  name: tags
  type: array
provider_name: Banuba
provider_slug: banuba
schema_file: json-schema/areffect-schema.json
slug: areffect
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/banuba/json-schema/areffect-schema.json\",\n  \"title\": \"AREffect\",\n  \"description\": \"A Banuba augmented reality effect that can be applied to a face in a video frame.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"effectId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the AR effect.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the effect.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category of the effect.\",\n      \"enum\": [\"mask\", \"filter\", \"beauty\", \"makeup\", \"accessory\", \"background\", \"avatar\"]\n    },\n    \"previewUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of a preview image for the effect.\"\n    },\n    \"effectUrl\": {\n      \"type\": \"\
  string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the effect bundle file.\"\n    },\n    \"platforms\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"iOS\", \"Android\", \"Web\", \"Windows\", \"macOS\", \"Unity\", \"Flutter\", \"React Native\"]\n      },\n      \"description\": \"Platforms supported by this effect.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags describing the effect.\"\n    }\n  },\n  \"required\": [\"effectId\", \"name\", \"category\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/banuba/refs/heads/main/json-schema/areffect-schema.json
tags:
- AR
- Augmented Reality
- Beauty
- Face Recognition
- Facial
- SDK
- Video
title: AREffect
---
