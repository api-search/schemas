---
description: A participant's submission to a DeepRacer leaderboard including race performance.
layout: schema
name: LeaderboardSubmission
properties_list:
- description: Unique identifier for this submission.
  name: leaderboardSubmissionId
  type: string
- description: The participant's alias or username.
  name: participantName
  type: string
- description: The ARN of the model submitted for evaluation.
  name: modelArn
  type: string
- description: The participant's current rank on the leaderboard.
  name: rank
  type: integer
- description: The participant's best single lap time in seconds.
  name: lapTime
  type: number
- description: The participant's average lap time.
  name: avgLapTime
  type: number
provider_name: Amazon DeepRacer
provider_slug: amazon-deepracer
schema_file: json-schema/leaderboard-submission-schema.json
slug: leaderboard-submission
source_filename: leaderboard-submission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deepracer/json-schema/leaderboard-submission-schema.json\",\n  \"title\": \"LeaderboardSubmission\",\n  \"description\": \"A participant's submission to a DeepRacer leaderboard including race performance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"leaderboardSubmissionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this submission.\"\n    },\n    \"participantName\": {\n      \"type\": \"string\",\n      \"description\": \"The participant's alias or username.\"\n    },\n    \"modelArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the model submitted for evaluation.\"\n    },\n    \"rank\": {\n      \"type\": \"integer\",\n      \"description\": \"The participant's current rank on the leaderboard.\"\n    },\n    \"lapTime\": {\n      \"type\": \"number\",\n      \"description\": \"\
  The participant's best single lap time in seconds.\"\n    },\n    \"avgLapTime\": {\n      \"type\": \"number\",\n      \"description\": \"The participant's average lap time.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deepracer/refs/heads/main/json-schema/leaderboard-submission-schema.json
tags:
- Autonomous Vehicles
- Machine Learning
- Reinforcement Learning
- Robotics
title: LeaderboardSubmission
---
