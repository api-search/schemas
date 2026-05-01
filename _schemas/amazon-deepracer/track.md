---
description: A virtual or physical racing track used for DeepRacer training and evaluation.
layout: schema
name: Track
properties_list:
- description: The ARN uniquely identifying the racing track.
  name: arn
  type: string
- description: The display name of the track.
  name: name
  type: string
- description: The classification type of the track.
  name: trackType
  type: string
- description: The size category of the track.
  name: trackDimension
  type: string
provider_name: Amazon DeepRacer
provider_slug: amazon-deepracer
schema_file: json-schema/track-schema.json
slug: track
source_filename: track-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deepracer/json-schema/track-schema.json\",\n  \"title\": \"Track\",\n  \"description\": \"A virtual or physical racing track used for DeepRacer training and evaluation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN uniquely identifying the racing track.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the track.\"\n    },\n    \"trackType\": {\n      \"type\": \"string\",\n      \"description\": \"The classification type of the track.\"\n    },\n    \"trackDimension\": {\n      \"type\": \"string\",\n      \"description\": \"The size category of the track.\",\n      \"enum\": [\n        \"REGULAR\",\n        \"WIDE\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deepracer/refs/heads/main/json-schema/track-schema.json
tags:
- Autonomous Vehicles
- Machine Learning
- Reinforcement Learning
- Robotics
title: Track
---
