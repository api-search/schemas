---
description: A show (production) in OpenCue
layout: schema
name: Show
properties_list:
- description: Unique show identifier
  name: id
  type: string
- description: Show name
  name: name
  type: string
- description: Whether the show is currently active
  name: active
  type: boolean
- description: Default minimum cores for jobs in this show
  name: defaultMinCores
  type: integer
- description: Default maximum cores for jobs in this show
  name: defaultMaxCores
  type: integer
provider_name: Academy Software Foundation
provider_slug: academy-software-foundation
schema_file: json-schema/opencue-show-schema.json
slug: opencue-show
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/json-schema/opencue-show-schema.json\",\n  \"title\": \"Show\",\n  \"description\": \"A show (production) in OpenCue\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique show identifier\",\n      \"example\": \"show-abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Show name\",\n      \"example\": \"feature_film_2026\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the show is currently active\",\n      \"example\": true\n    },\n    \"defaultMinCores\": {\n      \"type\": \"integer\",\n      \"description\": \"Default minimum cores for jobs in this show\",\n      \"example\": 100\n    },\n    \"defaultMaxCores\": {\n      \"type\": \"integer\",\n \
  \     \"description\": \"Default maximum cores for jobs in this show\",\n      \"example\": 5000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/json-schema/opencue-show-schema.json
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
title: Show
---
