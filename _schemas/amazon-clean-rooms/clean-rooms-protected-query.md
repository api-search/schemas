---
description: Represents a protected query executed within a Clean Rooms collaboration.
layout: schema
name: ProtectedQuery
properties_list:
- description: The unique ID of the protected query.
  name: id
  type: string
- description: The ID of the membership.
  name: membershipId
  type: string
- description: The ARN of the membership.
  name: membershipArn
  type: string
- description: The time when the query was created.
  name: createTime
  type: string
- description: The status of the protected query.
  name: status
  type: string
provider_name: Amazon Clean Rooms
provider_slug: amazon-clean-rooms
schema_file: json-schema/clean-rooms-protected-query-schema.json
slug: clean-rooms-protected-query
source_filename: clean-rooms-protected-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-protected-query-schema.json\",\n  \"title\": \"ProtectedQuery\",\n  \"description\": \"Represents a protected query executed within a Clean Rooms collaboration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of the protected query.\",\n      \"example\": \"query-abc12345\"\n    },\n    \"membershipId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the membership.\"\n    },\n    \"membershipArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the membership.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the query was created.\"\n    },\n    \"status\": {\n      \"type\": \"\
  string\",\n      \"enum\": [\n        \"SUBMITTED\",\n        \"STARTED\",\n        \"CANCELLED\",\n        \"CANCELLING\",\n        \"FAILED\",\n        \"SUCCESS\",\n        \"TIMED_OUT\"\n      ],\n      \"description\": \"The status of the protected query.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-protected-query-schema.json
tags:
- Clean Rooms
- Data Collaboration
- Privacy
- Analytics
- Marketing
title: ProtectedQuery
---
