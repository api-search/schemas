---
description: A layer within a render job
layout: schema
name: Layer
properties_list:
- description: Unique layer identifier
  name: id
  type: string
- description: Layer name
  name: name
  type: string
- description: Layer type
  name: type
  type: string
- description: Layer state
  name: state
  type: string
- description: Minimum cores required per frame
  name: minCores
  type: integer
- description: Maximum cores allowed per frame
  name: maxCores
  type: integer
- description: Whether frames can run multi-threaded
  name: threadable
  type: boolean
- description: Total number of frames in this layer
  name: totalFrames
  type: integer
- description: Number of completed frames in this layer
  name: doneFrames
  type: integer
provider_name: Academy Software Foundation
provider_slug: academy-software-foundation
schema_file: json-schema/opencue-layer-schema.json
slug: opencue-layer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/json-schema/opencue-layer-schema.json\",\n  \"title\": \"Layer\",\n  \"description\": \"A layer within a render job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique layer identifier\",\n      \"example\": \"layer-ghi789\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Layer name\",\n      \"example\": \"render\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Layer type\",\n      \"example\": \"RENDER\",\n      \"enum\": [\n        \"RENDER\",\n        \"UTIL\"\n      ]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Layer state\",\n      \"example\": \"RUNNING\"\n    },\n    \"minCores\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"Minimum cores required per frame\",\n      \"example\": 100\n    },\n    \"maxCores\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum cores allowed per frame\",\n      \"example\": 2000\n    },\n    \"threadable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether frames can run multi-threaded\",\n      \"example\": false\n    },\n    \"totalFrames\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of frames in this layer\",\n      \"example\": 100\n    },\n    \"doneFrames\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of completed frames in this layer\",\n      \"example\": 45\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/json-schema/opencue-layer-schema.json
tags:
- Animation
- Color Management
- Film
- Linux Foundation
- Open Source
- Rendering
- Standards
- Visual Effects
- VFX
title: Layer
---
