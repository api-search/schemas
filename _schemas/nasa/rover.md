---
description: A NASA Mars rover.
layout: schema
name: Mars Rover
properties_list:
- description: Unique identifier for the rover.
  name: id
  type: integer
- description: Name of the rover (e.g. Curiosity, Opportunity, Spirit).
  name: name
  type: string
- description: Date the rover landed on Mars.
  name: landing_date
  type: string
- description: Date the rover was launched from Earth.
  name: launch_date
  type: string
- description: Current mission status.
  name: status
  type: string
provider_name: NASA
provider_slug: nasa
schema_file: json-schema/rover.json
slug: rover
source_filename: rover.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/nasa/blob/main/json-schema/rover.json\",\n  \"title\": \"Mars Rover\",\n  \"description\": \"A NASA Mars rover.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the rover.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the rover (e.g. Curiosity, Opportunity, Spirit).\"\n    },\n    \"landing_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the rover landed on Mars.\"\n    },\n    \"launch_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the rover was launched from Earth.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"complete\"],\n      \"description\": \"Current mission status.\"\n   \
  \ }\n  },\n  \"required\": [\"id\", \"name\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/json-schema/rover.json
tags:
- Government
- Science
- Space
title: Mars Rover
---
