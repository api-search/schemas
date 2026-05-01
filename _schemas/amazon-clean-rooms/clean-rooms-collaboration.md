---
description: Represents an AWS Clean Rooms collaboration workspace.
layout: schema
name: Collaboration
properties_list:
- description: The unique ID of the collaboration.
  name: id
  type: string
- description: The ARN of the collaboration.
  name: arn
  type: string
- description: A human-readable identifier for the collaboration.
  name: name
  type: string
- description: A description of the collaboration.
  name: description
  type: string
- description: The account ID of the creator.
  name: creatorAccountId
  type: string
- description: The display name of the collaboration creator.
  name: creatorDisplayName
  type: string
- description: The time when the collaboration was created.
  name: createTime
  type: string
- description: The time when the collaboration was last updated.
  name: updateTime
  type: string
- description: Whether query logs are enabled.
  name: queryLogStatus
  type: string
provider_name: Amazon Clean Rooms
provider_slug: amazon-clean-rooms
schema_file: json-schema/clean-rooms-collaboration-schema.json
slug: clean-rooms-collaboration
source_filename: clean-rooms-collaboration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-collaboration-schema.json\",\n  \"title\": \"Collaboration\",\n  \"description\": \"Represents an AWS Clean Rooms collaboration workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of the collaboration.\",\n      \"example\": \"collab-abc12345\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the collaboration.\",\n      \"example\": \"arn:aws:cleanrooms:us-east-1:123456789012:collaboration/collab-abc12345\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable identifier for the collaboration.\",\n      \"example\": \"Marketing Analytics Collaboration\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"A description of the collaboration.\",\n      \"example\": \"Collaborative analytics for marketing measurement\"\n    },\n    \"creatorAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The account ID of the creator.\",\n      \"example\": \"123456789012\"\n    },\n    \"creatorDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the collaboration creator.\",\n      \"example\": \"Acme Corp\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the collaboration was created.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the collaboration was last updated.\"\n    },\n    \"queryLogStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENABLED\",\n        \"DISABLED\"\n      ],\n      \"description\": \"Whether query logs\
  \ are enabled.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-collaboration-schema.json
tags:
- Clean Rooms
- Data Collaboration
- Privacy
- Analytics
- Marketing
title: Collaboration
---
