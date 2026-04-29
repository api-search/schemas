---
description: Error response returned when an API request fails.
layout: schema
name: Error
properties_list:
- description: A human-readable description of the error.
  name: message
  type: string
- description: An error code identifying the type of failure.
  name: code
  type: string
provider_name: Amazon DeepRacer
provider_slug: amazon-deepracer
schema_file: json-schema/error-schema.json
slug: error
source_filename: error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deepracer/json-schema/error-schema.json\",\n  \"title\": \"Error\",\n  \"description\": \"Error response returned when an API request fails.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the error.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"An error code identifying the type of failure.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deepracer/refs/heads/main/json-schema/error-schema.json
tags:
- Autonomous Vehicles
- AWS
- Machine Learning
- Reinforcement Learning
- Robotics
title: Error
---
