---
description: An entry in the Helix Swarm activity stream recording an action performed by a user.
layout: schema
name: Activity
properties_list:
- description: The unique activity entry identifier.
  name: id
  type: integer
- description: A past-tense description of the action performed.
  name: action
  type: string
- description: The related changelist ID, if applicable.
  name: change
  type: integer
- description: The date and time the activity occurred.
  name: date
  type: string
- description: Contextual information about the activity.
  name: description
  type: string
- description: A URL linking to the activity target.
  name: link
  type: string
- description: The activity streams this entry appears in.
  name: streams
  type: array
- description: The object that received the action.
  name: target
  type: string
- description: An associated comment thread topic.
  name: topic
  type: string
- description: The activity type classification.
  name: type
  type: string
- description: The username of the user who performed the action.
  name: user
  type: string
provider_name: Perforce
provider_slug: perforce
schema_file: json-schema/perforce-helix-swarm-activity-schema.json
slug: perforce-helix-swarm-activity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Activity\",\n  \"type\": \"object\",\n  \"description\": \"An entry in the Helix Swarm activity stream recording an action performed by a user.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique activity entry identifier.\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"A past-tense description of the action performed.\"\n    },\n    \"change\": {\n      \"type\": \"integer\",\n      \"description\": \"The related changelist ID, if applicable.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the activity occurred.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Contextual information about the activity.\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"description\": \"A URL linking to the activity\
  \ target.\"\n    },\n    \"streams\": {\n      \"type\": \"array\",\n      \"description\": \"The activity streams this entry appears in.\"\n    },\n    \"target\": {\n      \"type\": \"string\",\n      \"description\": \"The object that received the action.\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"An associated comment thread topic.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The activity type classification.\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"The username of the user who performed the action.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/json-schema/perforce-helix-swarm-activity-schema.json
tags: []
title: Activity
---
