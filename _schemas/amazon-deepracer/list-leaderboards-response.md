---
description: Response containing a list of DeepRacer leaderboards.
layout: schema
name: ListLeaderboardsResponse
properties_list:
- description: List of leaderboards.
  name: leaderboards
  type: array
- description: Token for retrieving the next page of results.
  name: nextToken
  type: string
provider_name: Amazon DeepRacer
provider_slug: amazon-deepracer
schema_file: json-schema/list-leaderboards-response-schema.json
slug: list-leaderboards-response
source_filename: list-leaderboards-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deepracer/json-schema/list-leaderboards-response-schema.json\",\n  \"title\": \"ListLeaderboardsResponse\",\n  \"description\": \"Response containing a list of DeepRacer leaderboards.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"leaderboards\": {\n      \"type\": \"array\",\n      \"description\": \"List of leaderboards.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for retrieving the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deepracer/refs/heads/main/json-schema/list-leaderboards-response-schema.json
tags:
- Autonomous Vehicles
- Machine Learning
- Reinforcement Learning
- Robotics
title: ListLeaderboardsResponse
---
