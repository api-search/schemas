---
description: A camera mounted on a NASA Mars rover.
layout: schema
name: Rover Camera
properties_list:
- description: Unique identifier for the camera.
  name: id
  type: integer
- description: Abbreviated name of the camera (e.g. FHAZ, RHAZ, MAST).
  name: name
  type: string
- description: ID of the rover this camera belongs to.
  name: rover_id
  type: integer
- description: Full descriptive name of the camera.
  name: full_name
  type: string
provider_name: NASA
provider_slug: nasa
schema_file: json-schema/camera.json
slug: camera
source_filename: camera.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/nasa/blob/main/json-schema/camera.json\",\n  \"title\": \"Rover Camera\",\n  \"description\": \"A camera mounted on a NASA Mars rover.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the camera.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Abbreviated name of the camera (e.g. FHAZ, RHAZ, MAST).\"\n    },\n    \"rover_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the rover this camera belongs to.\"\n    },\n    \"full_name\": {\n      \"type\": \"string\",\n      \"description\": \"Full descriptive name of the camera.\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"full_name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/json-schema/camera.json
tags:
- Government
- Science
- Space
title: Rover Camera
---
