---
description: A DeepRacer racing leaderboard where participants submit model performances.
layout: schema
name: Leaderboard
properties_list:
- description: The ARN uniquely identifying the leaderboard.
  name: arn
  type: string
- description: The display name of the leaderboard.
  name: name
  type: string
- description: Current status.
  name: status
  type: string
- description: Timestamp when submissions close.
  name: submissionClosureTime
  type: string
- description: Whether this leaderboard qualifies participants for championship events.
  name: isQualifier
  type: boolean
- description: The type of track used for this leaderboard.
  name: trackType
  type: string
- description: Minimum number of consecutive laps required.
  name: minimumCountOfLaps
  type: integer
provider_name: Amazon DeepRacer
provider_slug: amazon-deepracer
schema_file: json-schema/leaderboard-schema.json
slug: leaderboard
source_filename: leaderboard-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deepracer/json-schema/leaderboard-schema.json\",\n  \"title\": \"Leaderboard\",\n  \"description\": \"A DeepRacer racing leaderboard where participants submit model performances.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN uniquely identifying the leaderboard.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the leaderboard.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status.\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"EXPIRED\"\n      ]\n    },\n    \"submissionClosureTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when submissions close.\"\n    },\n    \"isQualifier\": {\n      \"type\": \"boolean\",\n\
  \      \"description\": \"Whether this leaderboard qualifies participants for championship events.\"\n    },\n    \"trackType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of track used for this leaderboard.\"\n    },\n    \"minimumCountOfLaps\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum number of consecutive laps required.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deepracer/refs/heads/main/json-schema/leaderboard-schema.json
tags:
- Autonomous Vehicles
- AWS
- Machine Learning
- Reinforcement Learning
- Robotics
title: Leaderboard
---
