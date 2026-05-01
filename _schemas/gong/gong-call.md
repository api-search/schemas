---
description: Represents a call record in the Gong platform, including metadata, participants, timing, and media information.
layout: schema
name: Gong Call
properties_list:
- description: Unique numeric identifier for the call (up to 20 digits).
  name: id
  type: string
- description: The title or subject of the call.
  name: title
  type: string
- description: URL to the call in the Gong web application.
  name: url
  type: string
- description: Scheduled start time of the call in ISO-8601 format.
  name: scheduled
  type: string
- description: Actual start time of the call in ISO-8601 format.
  name: started
  type: string
- description: Duration of the call in seconds.
  name: duration
  type: number
- description: The direction of the call.
  name: direction
  type: string
- description: Whether the call was internal or external.
  name: scope
  type: string
- description: The type of media recorded.
  name: media
  type: string
- description: The detected language of the call.
  name: language
  type: string
- description: The workspace identifier the call belongs to.
  name: workspaceId
  type: string
- description: The Gong user ID of the primary user on the call.
  name: primaryUserId
  type: string
- description: The participants in the call.
  name: parties
  type: array
provider_name: Gong
provider_slug: gong
schema_file: json-schema/gong-call-schema.json
slug: gong-call
source_filename: gong-call-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gong/blob/main/json-schema/gong-call-schema.json\",\n  \"title\": \"Gong Call\",\n  \"description\": \"Represents a call record in the Gong platform, including metadata, participants, timing, and media information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique numeric identifier for the call (up to 20 digits).\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title or subject of the call.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the call in the Gong web application.\"\n    },\n    \"scheduled\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scheduled start time of the call in ISO-8601 format.\"\n    },\n    \"started\": {\n   \
  \   \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Actual start time of the call in ISO-8601 format.\"\n    },\n    \"duration\": {\n      \"type\": \"number\",\n      \"description\": \"Duration of the call in seconds.\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"enum\": [\"Inbound\", \"Outbound\", \"Conference\", \"Unknown\"],\n      \"description\": \"The direction of the call.\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"enum\": [\"Internal\", \"External\", \"Unknown\"],\n      \"description\": \"Whether the call was internal or external.\"\n    },\n    \"media\": {\n      \"type\": \"string\",\n      \"enum\": [\"Video\", \"Audio\"],\n      \"description\": \"The type of media recorded.\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"The detected language of the call.\"\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"description\": \"The workspace\
  \ identifier the call belongs to.\"\n    },\n    \"primaryUserId\": {\n      \"type\": \"string\",\n      \"description\": \"The Gong user ID of the primary user on the call.\"\n    },\n    \"parties\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CallParty\"\n      },\n      \"description\": \"The participants in the call.\"\n    }\n  },\n  \"required\": [\"id\"],\n  \"$defs\": {\n    \"CallParty\": {\n      \"type\": \"object\",\n      \"description\": \"A participant in a Gong call.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the party.\"\n        },\n        \"emailAddress\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address of the party.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the party.\"\n        },\n        \"title\": {\n \
  \         \"type\": \"string\",\n          \"description\": \"Job title of the party.\"\n        },\n        \"userId\": {\n          \"type\": \"string\",\n          \"description\": \"Gong user ID if the party is a Gong user.\"\n        },\n        \"speakerId\": {\n          \"type\": \"string\",\n          \"description\": \"Speaker identifier within the call.\"\n        },\n        \"affiliation\": {\n          \"type\": \"string\",\n          \"enum\": [\"Internal\", \"External\", \"Unknown\"],\n          \"description\": \"Whether the party is internal or external.\"\n        },\n        \"phoneNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Phone number of the party.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/json-schema/gong-call-schema.json
tags: []
title: Gong Call
---
