---
description: A basket is a JSON container stored within a pantry.
layout: schema
name: Basket
properties_list:
- description: Name of the basket.
  name: name
  type: string
- description: Time-to-live in seconds before basket expiry.
  name: ttl
  type: integer
- description: Free-form JSON contents of the basket.
  name: contents
  type: object
provider_name: Pantry
provider_slug: pantry
schema_file: json-schema/basket.json
slug: basket
source_filename: basket.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/pantry/refs/heads/main/json-schema/basket.json\",\n  \"title\": \"Basket\",\n  \"description\": \"A basket is a JSON container stored within a pantry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the basket.\"\n    },\n    \"ttl\": {\n      \"type\": \"integer\",\n      \"description\": \"Time-to-live in seconds before basket expiry.\"\n    },\n    \"contents\": {\n      \"type\": \"object\",\n      \"description\": \"Free-form JSON contents of the basket.\",\n      \"additionalProperties\": true\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/pantry/refs/heads/main/json-schema/basket.json
tags:
- Data Storage
- Developer Tools
- JSON
title: Basket
---
