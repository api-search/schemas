---
description: Request body for creating a collaboration.
layout: schema
name: CreateCollaborationRequest
properties_list:
- description: The display name for a collaboration.
  name: name
  type: string
- description: A description of the collaboration.
  name: description
  type: string
- description: A list of initial members for the collaboration.
  name: members
  type: array
- description: The display name of the collaboration creator.
  name: creatorDisplayName
  type: string
- description: The abilities granted to the collaboration creator.
  name: creatorMemberAbilities
  type: array
- description: An indicator as to whether query logging has been enabled or disabled.
  name: queryLogStatus
  type: string
provider_name: Amazon Clean Rooms
provider_slug: amazon-clean-rooms
schema_file: json-schema/clean-rooms-create-collaboration-request-schema.json
slug: clean-rooms-create-collaboration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-create-collaboration-request-schema.json\",\n  \"title\": \"CreateCollaborationRequest\",\n  \"description\": \"Request body for creating a collaboration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name for a collaboration.\",\n      \"example\": \"Marketing Analytics Collaboration\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the collaboration.\"\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"A list of initial members for the collaboration.\"\n    },\n    \"creatorDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display\
  \ name of the collaboration creator.\"\n    },\n    \"creatorMemberAbilities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The abilities granted to the collaboration creator.\"\n    },\n    \"queryLogStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENABLED\",\n        \"DISABLED\"\n      ],\n      \"description\": \"An indicator as to whether query logging has been enabled or disabled.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"members\",\n    \"creatorDisplayName\",\n    \"creatorMemberAbilities\",\n    \"queryLogStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-create-collaboration-request-schema.json
tags:
- AWS
- Clean Rooms
- Data Collaboration
- Privacy
- Analytics
- Marketing
title: CreateCollaborationRequest
---
