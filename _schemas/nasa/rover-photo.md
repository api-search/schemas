---
description: A photo taken by a NASA Mars rover.
layout: schema
name: Mars Rover Photo
properties_list:
- description: Unique identifier for the photo.
  name: id
  type: integer
- description: Martian sol (day) on which the photo was taken.
  name: sol
  type: integer
- description: ''
  name: camera
  type: object
- description: URL of the image.
  name: img_src
  type: string
- description: Earth date when the photo was taken.
  name: earth_date
  type: string
- description: ''
  name: rover
  type: object
provider_name: NASA
provider_slug: nasa
schema_file: json-schema/rover-photo.json
slug: rover-photo
source_filename: rover-photo.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/nasa/blob/main/json-schema/rover-photo.json\",\n  \"title\": \"Mars Rover Photo\",\n  \"description\": \"A photo taken by a NASA Mars rover.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the photo.\"\n    },\n    \"sol\": {\n      \"type\": \"integer\",\n      \"description\": \"Martian sol (day) on which the photo was taken.\"\n    },\n    \"camera\": {\n      \"$ref\": \"camera.json\"\n    },\n    \"img_src\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the image.\"\n    },\n    \"earth_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Earth date when the photo was taken.\"\n    },\n    \"rover\": {\n      \"$ref\": \"rover.json\"\n    }\n  },\n  \"required\": [\"id\", \"sol\"\
  , \"img_src\", \"earth_date\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/json-schema/rover-photo.json
tags:
- Government
- Science
- Space
title: Mars Rover Photo
---
