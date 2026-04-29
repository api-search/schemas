---
description: Represents a configured table in Clean Rooms.
layout: schema
name: ConfiguredTable
properties_list:
- description: The unique ID of the configured table.
  name: id
  type: string
- description: The ARN of the configured table.
  name: arn
  type: string
- description: A human-readable name for the configured table.
  name: name
  type: string
- description: A description of the configured table.
  name: description
  type: string
- description: The time when the configured table was created.
  name: createTime
  type: string
- description: The time when the configured table was last updated.
  name: updateTime
  type: string
- description: The analysis method for the configured table.
  name: analysisMethod
  type: string
provider_name: Amazon Clean Rooms
provider_slug: amazon-clean-rooms
schema_file: json-schema/clean-rooms-configured-table-schema.json
slug: clean-rooms-configured-table
source_filename: clean-rooms-configured-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-configured-table-schema.json\",\n  \"title\": \"ConfiguredTable\",\n  \"description\": \"Represents a configured table in Clean Rooms.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of the configured table.\",\n      \"example\": \"table-abc12345\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the configured table.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable name for the configured table.\",\n      \"example\": \"Customer Segments Table\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the configured table.\"\n    },\n    \"createTime\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the configured table was created.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the configured table was last updated.\"\n    },\n    \"analysisMethod\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DIRECT_QUERY\"\n      ],\n      \"description\": \"The analysis method for the configured table.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-configured-table-schema.json
tags:
- AWS
- Clean Rooms
- Data Collaboration
- Privacy
- Analytics
- Marketing
title: ConfiguredTable
---
