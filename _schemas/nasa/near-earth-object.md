---
description: A near-Earth asteroid tracked by NASA's NeoWs service.
layout: schema
name: Near Earth Object
properties_list:
- description: Unique identifier for the NEO.
  name: id
  type: string
- description: NEO reference identifier.
  name: neo_reference_id
  type: string
- description: Name or designation of the asteroid.
  name: name
  type: string
- description: URL to the NASA JPL page for this object.
  name: nasa_jpl_url
  type: string
- description: Absolute magnitude (H) of the asteroid.
  name: absolute_magnitude_h
  type: number
- description: Estimated diameter in various units.
  name: estimated_diameter
  type: object
- description: Whether the asteroid is classified as potentially hazardous.
  name: is_potentially_hazardous_asteroid
  type: boolean
- description: List of close approach events.
  name: close_approach_data
  type: array
- description: Whether this object is tracked by the Sentry impact monitoring system.
  name: is_sentry_object
  type: boolean
provider_name: NASA
provider_slug: nasa
schema_file: json-schema/near-earth-object.json
slug: near-earth-object
source_filename: near-earth-object.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/nasa/blob/main/json-schema/near-earth-object.json\",\n  \"title\": \"Near Earth Object\",\n  \"description\": \"A near-Earth asteroid tracked by NASA's NeoWs service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the NEO.\"\n    },\n    \"neo_reference_id\": {\n      \"type\": \"string\",\n      \"description\": \"NEO reference identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name or designation of the asteroid.\"\n    },\n    \"nasa_jpl_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the NASA JPL page for this object.\"\n    },\n    \"absolute_magnitude_h\": {\n      \"type\": \"number\",\n      \"description\": \"Absolute magnitude (H) of the asteroid.\"\n    },\n    \"\
  estimated_diameter\": {\n      \"type\": \"object\",\n      \"description\": \"Estimated diameter in various units.\",\n      \"properties\": {\n        \"kilometers\": { \"$ref\": \"#/$defs/diameterRange\" },\n        \"meters\": { \"$ref\": \"#/$defs/diameterRange\" },\n        \"miles\": { \"$ref\": \"#/$defs/diameterRange\" },\n        \"feet\": { \"$ref\": \"#/$defs/diameterRange\" }\n      }\n    },\n    \"is_potentially_hazardous_asteroid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the asteroid is classified as potentially hazardous.\"\n    },\n    \"close_approach_data\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"close-approach.json\" },\n      \"description\": \"List of close approach events.\"\n    },\n    \"is_sentry_object\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this object is tracked by the Sentry impact monitoring system.\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"is_potentially_hazardous_asteroid\"\
  ],\n  \"$defs\": {\n    \"diameterRange\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"estimated_diameter_min\": { \"type\": \"number\" },\n        \"estimated_diameter_max\": { \"type\": \"number\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/json-schema/near-earth-object.json
tags:
- Government
- Science
- Space
title: Near Earth Object
---
