---
description: Response containing a list of available racing tracks.
layout: schema
name: ListTracksResponse
properties_list:
- description: List of racing tracks.
  name: tracks
  type: array
- description: Token for retrieving the next page of results.
  name: nextToken
  type: string
provider_name: Amazon DeepRacer
provider_slug: amazon-deepracer
schema_file: json-schema/list-tracks-response-schema.json
slug: list-tracks-response
source_filename: list-tracks-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deepracer/json-schema/list-tracks-response-schema.json\",\n  \"title\": \"ListTracksResponse\",\n  \"description\": \"Response containing a list of available racing tracks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tracks\": {\n      \"type\": \"array\",\n      \"description\": \"List of racing tracks.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for retrieving the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deepracer/refs/heads/main/json-schema/list-tracks-response-schema.json
tags:
- Autonomous Vehicles
- AWS
- Machine Learning
- Reinforcement Learning
- Robotics
title: ListTracksResponse
---
