---
description: A pantry account container with metadata and a list of baskets.
layout: schema
name: Pantry
properties_list:
- description: Display name for the pantry.
  name: name
  type: string
- description: Description of the pantry.
  name: description
  type: string
- description: ''
  name: errors
  type: array
- description: ''
  name: notifications
  type: boolean
- description: ''
  name: percentFull
  type: integer
- description: ''
  name: baskets
  type: array
provider_name: Pantry
provider_slug: pantry
schema_file: json-schema/pantry.json
slug: pantry
source_filename: pantry.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/pantry/refs/heads/main/json-schema/pantry.json\",\n  \"title\": \"Pantry\",\n  \"description\": \"A pantry account container with metadata and a list of baskets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the pantry.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the pantry.\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"notifications\": {\n      \"type\": \"boolean\"\n    },\n    \"percentFull\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"baskets\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"basket.json\" }\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/pantry/refs/heads/main/json-schema/pantry.json
tags:
- Data Storage
- Developer Tools
- JSON
title: Pantry
---
