---
description: DmEvent schema from X API v2
layout: schema
name: DmEvent
properties_list:
- description: Specifies the type of attachments (if any) present in this DM.
  name: attachments
  type: object
- description: ''
  name: cashtags
  type: array
- description: ''
  name: created_at
  type: string
- description: Unique identifier of a DM conversation. This can either be a numeric string, or a pair of numeric strings separated by a '-' character in the case of one-on-one DM Conversations.
  name: dm_conversation_id
  type: string
- description: ''
  name: event_type
  type: string
- description: ''
  name: hashtags
  type: array
- description: Unique identifier of a DM Event.
  name: id
  type: string
- description: ''
  name: mentions
  type: array
- description: A list of participants for a ParticipantsJoin or ParticipantsLeave event_type.
  name: participant_ids
  type: array
- description: A list of Posts this DM refers to.
  name: referenced_tweets
  type: array
- description: Unique identifier of this User. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.
  name: sender_id
  type: string
- description: ''
  name: text
  type: string
- description: ''
  name: urls
  type: array
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-dm-event-schema.json
slug: x-api-dm-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-dm-event-schema.json\",\n  \"title\": \"DmEvent\",\n  \"description\": \"DmEvent schema from X API v2\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attachments\": {\n      \"type\": \"object\",\n      \"description\": \"Specifies the type of attachments (if any) present in this DM.\",\n      \"properties\": {\n        \"card_ids\": {\n          \"type\": \"array\",\n          \"description\": \"A list of card IDs (if cards are attached).\",\n          \"minItems\": 1,\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"media_keys\": {\n          \"type\": \"array\",\n          \"description\": \"A list of Media Keys for each one of the media attachments (if media are attached).\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\"\
  : \"#/components/schemas/MediaKey\"\n          }\n        }\n      }\n    },\n    \"cashtags\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CashtagEntity\"\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"dm_conversation_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of a DM conversation. This can either be a numeric string, or a pair of numeric strings separated by a '-' character in the case of one-on-one DM Conversations.\",\n      \"pattern\": \"^([0-9]{1,19}-[0-9]{1,19}|[0-9]{15,19})$\",\n      \"example\": \"123123123-456456456\"\n    },\n    \"event_type\": {\n      \"type\": \"string\",\n      \"example\": \"MessageCreate\"\n    },\n    \"hashtags\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/HashtagEntity\"\n      }\n    },\n    \"id\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of a DM Event.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"1146654567674912769\"\n    },\n    \"mentions\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MentionEntity\"\n      }\n    },\n    \"participant_ids\": {\n      \"type\": \"array\",\n      \"description\": \"A list of participants for a ParticipantsJoin or ParticipantsLeave event_type.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UserId\"\n      }\n    },\n    \"referenced_tweets\": {\n      \"type\": \"array\",\n      \"description\": \"A list of Posts this DM refers to.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"id\"\n        ],\n        \"properties\": {\n          \"id\": {\n            \"$ref\": \"#/components/schemas/TweetId\"\n          }\n\
  \        }\n      }\n    },\n    \"sender_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of this User. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"2244994945\"\n    },\n    \"text\": {\n      \"type\": \"string\"\n    },\n    \"urls\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UrlEntityDm\"\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"event_type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-dm-event-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: DmEvent
---
