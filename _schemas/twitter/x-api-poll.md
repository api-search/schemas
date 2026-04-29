---
description: Represent a Poll attached to a Tweet.
layout: schema
name: Poll
properties_list:
- description: ''
  name: duration_minutes
  type: integer
- description: ''
  name: end_datetime
  type: string
- description: Unique identifier of this poll.
  name: id
  type: string
- description: ''
  name: options
  type: array
- description: ''
  name: voting_status
  type: string
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-poll-schema.json
slug: x-api-poll
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-poll-schema.json\",\n  \"title\": \"Poll\",\n  \"description\": \"Represent a Poll attached to a Tweet.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"duration_minutes\": {\n      \"type\": \"integer\",\n      \"minimum\": 5,\n      \"maximum\": 10080,\n      \"format\": \"int32\"\n    },\n    \"end_datetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of this poll.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"1365059861688410112\"\n    },\n    \"options\": {\n      \"type\": \"array\",\n      \"minItems\": 2,\n      \"maxItems\": 4,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PollOption\"\n      }\n    },\n    \"voting_status\": {\n      \"type\"\
  : \"string\",\n      \"enum\": [\n        \"open\",\n        \"closed\"\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"options\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-poll-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: Poll
---
