---
description: Represents a member's participation in a Clean Rooms collaboration.
layout: schema
name: Membership
properties_list:
- description: The unique ID of the membership.
  name: id
  type: string
- description: The ARN of the membership.
  name: arn
  type: string
- description: The ARN of the collaboration.
  name: collaborationArn
  type: string
- description: The ID of the collaboration.
  name: collaborationId
  type: string
- description: The account ID of the collaboration creator.
  name: collaborationCreatorAccountId
  type: string
- description: The name of the collaboration.
  name: collaborationName
  type: string
- description: The status of the membership.
  name: status
  type: string
provider_name: Amazon Clean Rooms
provider_slug: amazon-clean-rooms
schema_file: json-schema/clean-rooms-membership-schema.json
slug: clean-rooms-membership
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-membership-schema.json\",\n  \"title\": \"Membership\",\n  \"description\": \"Represents a member's participation in a Clean Rooms collaboration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of the membership.\",\n      \"example\": \"member-abc12345\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the membership.\"\n    },\n    \"collaborationArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the collaboration.\"\n    },\n    \"collaborationId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the collaboration.\"\n    },\n    \"collaborationCreatorAccountId\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"The account ID of the collaboration creator.\"\n    },\n    \"collaborationName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the collaboration.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"COLLABORATION_DELETED\",\n        \"REMOVED\"\n      ],\n      \"description\": \"The status of the membership.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-membership-schema.json
tags:
- AWS
- Clean Rooms
- Data Collaboration
- Privacy
- Analytics
- Marketing
title: Membership
---
