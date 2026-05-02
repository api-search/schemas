---
description: A close approach event for a near-Earth object.
layout: schema
name: Close Approach
properties_list:
- description: Date of the close approach (YYYY-MM-DD).
  name: close_approach_date
  type: string
- description: Full date and time of close approach.
  name: close_approach_date_full
  type: string
- description: Epoch timestamp of the close approach.
  name: epoch_date_close_approach
  type: integer
- description: ''
  name: relative_velocity
  type: object
- description: ''
  name: miss_distance
  type: object
- description: The orbiting body for the close approach (e.g. Earth).
  name: orbiting_body
  type: string
provider_name: NASA
provider_slug: nasa
schema_file: json-schema/close-approach.json
slug: close-approach
source_filename: close-approach.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/nasa/blob/main/json-schema/close-approach.json\",\n  \"title\": \"Close Approach\",\n  \"description\": \"A close approach event for a near-Earth object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"close_approach_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the close approach (YYYY-MM-DD).\"\n    },\n    \"close_approach_date_full\": {\n      \"type\": \"string\",\n      \"description\": \"Full date and time of close approach.\"\n    },\n    \"epoch_date_close_approach\": {\n      \"type\": \"integer\",\n      \"description\": \"Epoch timestamp of the close approach.\"\n    },\n    \"relative_velocity\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"kilometers_per_second\": { \"type\": \"string\" },\n        \"kilometers_per_hour\": { \"type\": \"string\" },\n        \"miles_per_hour\"\
  : { \"type\": \"string\" }\n      }\n    },\n    \"miss_distance\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"astronomical\": { \"type\": \"string\" },\n        \"lunar\": { \"type\": \"string\" },\n        \"kilometers\": { \"type\": \"string\" },\n        \"miles\": { \"type\": \"string\" }\n      }\n    },\n    \"orbiting_body\": {\n      \"type\": \"string\",\n      \"description\": \"The orbiting body for the close approach (e.g. Earth).\"\n    }\n  },\n  \"required\": [\"close_approach_date\", \"orbiting_body\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/json-schema/close-approach.json
tags:
- Government
- Science
- Space
title: Close Approach
---
