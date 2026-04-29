---
description: Response containing leaderboard rankings and submissions.
layout: schema
name: ListLeaderboardSubmissionsResponse
properties_list:
- description: List of participant submissions.
  name: leaderboardSubmissions
  type: array
- description: Token for retrieving the next page of results.
  name: nextToken
  type: string
provider_name: Amazon DeepRacer
provider_slug: amazon-deepracer
schema_file: json-schema/list-leaderboard-submissions-response-schema.json
slug: list-leaderboard-submissions-response
source_filename: list-leaderboard-submissions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deepracer/json-schema/list-leaderboard-submissions-response-schema.json\",\n  \"title\": \"ListLeaderboardSubmissionsResponse\",\n  \"description\": \"Response containing leaderboard rankings and submissions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"leaderboardSubmissions\": {\n      \"type\": \"array\",\n      \"description\": \"List of participant submissions.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for retrieving the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deepracer/refs/heads/main/json-schema/list-leaderboard-submissions-response-schema.json
tags:
- Autonomous Vehicles
- AWS
- Machine Learning
- Reinforcement Learning
- Robotics
title: ListLeaderboardSubmissionsResponse
---
