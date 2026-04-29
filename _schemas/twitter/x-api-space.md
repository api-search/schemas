---
description: ''
layout: schema
name: Space
properties_list:
- description: Creation time of the Space.
  name: created_at
  type: string
- description: Unique identifier of this User. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.
  name: creator_id
  type: string
- description: End time of the Space.
  name: ended_at
  type: string
- description: The user ids for the hosts of the Space.
  name: host_ids
  type: array
- description: The unique identifier of this Space.
  name: id
  type: string
- description: An array of user ids for people who were invited to a Space.
  name: invited_user_ids
  type: array
- description: Denotes if the Space is a ticketed Space.
  name: is_ticketed
  type: boolean
- description: The language of the Space.
  name: lang
  type: string
- description: The number of participants in a Space.
  name: participant_count
  type: integer
- description: A date time stamp for when a Space is scheduled to begin.
  name: scheduled_start
  type: string
- description: An array of user ids for people who were speakers in a Space.
  name: speaker_ids
  type: array
- description: When the Space was started as a date string.
  name: started_at
  type: string
- description: The current state of the Space.
  name: state
  type: string
- description: The number of people who have either purchased a ticket or set a reminder for this Space.
  name: subscriber_count
  type: integer
- description: The title of the Space.
  name: title
  type: string
- description: The topics of a Space, as selected by its creator.
  name: topics
  type: array
- description: When the Space was last updated.
  name: updated_at
  type: string
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-space-schema.json
slug: x-api-space
source_filename: x-api-space-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-space-schema.json\",\n  \"title\": \"Space\",\n  \"description\": \"\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"Creation time of the Space.\",\n      \"format\": \"date-time\",\n      \"example\": \"2021-07-06T18:40:40.000Z\"\n    },\n    \"creator_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of this User. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"2244994945\"\n    },\n    \"ended_at\": {\n      \"type\": \"string\",\n      \"description\": \"End time of the Space.\",\n      \"format\": \"date-time\",\n      \"example\": \"2021-07-06T18:40:40.000Z\"\
  \n    },\n    \"host_ids\": {\n      \"type\": \"array\",\n      \"description\": \"The user ids for the hosts of the Space.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UserId\"\n      }\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of this Space.\",\n      \"pattern\": \"^[a-zA-Z0-9]{1,13}$\",\n      \"example\": \"1SLjjRYNejbKM\"\n    },\n    \"invited_user_ids\": {\n      \"type\": \"array\",\n      \"description\": \"An array of user ids for people who were invited to a Space.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UserId\"\n      }\n    },\n    \"is_ticketed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Denotes if the Space is a ticketed Space.\",\n      \"example\": \"false\"\n    },\n    \"lang\": {\n      \"type\": \"string\",\n      \"description\": \"The language of the Space.\",\n      \"example\": \"en\"\n    },\n    \"participant_count\": {\n      \"type\": \"\
  integer\",\n      \"description\": \"The number of participants in a Space.\",\n      \"format\": \"int32\",\n      \"example\": 10\n    },\n    \"scheduled_start\": {\n      \"type\": \"string\",\n      \"description\": \"A date time stamp for when a Space is scheduled to begin.\",\n      \"format\": \"date-time\",\n      \"example\": \"2021-07-06T18:40:40.000Z\"\n    },\n    \"speaker_ids\": {\n      \"type\": \"array\",\n      \"description\": \"An array of user ids for people who were speakers in a Space.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UserId\"\n      }\n    },\n    \"started_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the Space was started as a date string.\",\n      \"format\": \"date-time\",\n      \"example\": \"2021-7-14T04:35:55Z\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the Space.\",\n      \"enum\": [\n        \"live\",\n        \"scheduled\",\n        \"\
  ended\"\n      ],\n      \"example\": \"live\"\n    },\n    \"subscriber_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of people who have either purchased a ticket or set a reminder for this Space.\",\n      \"format\": \"int32\",\n      \"example\": 10\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Space.\",\n      \"example\": \"Spaces are Awesome\"\n    },\n    \"topics\": {\n      \"type\": \"array\",\n      \"description\": \"The topics of a Space, as selected by its creator.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"The X Topic object.\",\n        \"required\": [\n          \"id\",\n          \"name\"\n        ],\n        \"properties\": {\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"The description of the given topic.\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"An ID suitable for use in the REST API.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the given topic.\"\n          }\n        },\n        \"example\": {\n          \"description\": \"All about technology\",\n          \"id\": \"848920371311001600\",\n          \"name\": \"Technology\"\n        }\n      }\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the Space was last updated.\",\n      \"format\": \"date-time\",\n      \"example\": \"2021-7-14T04:35:55Z\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"state\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-space-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: Space
---
