---
description: A X List is a curated group of accounts.
layout: schema
name: List
properties_list:
- description: ''
  name: created_at
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: follower_count
  type: integer
- description: The unique identifier of this List.
  name: id
  type: string
- description: ''
  name: member_count
  type: integer
- description: The name of this List.
  name: name
  type: string
- description: Unique identifier of this User. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.
  name: owner_id
  type: string
- description: ''
  name: private
  type: boolean
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-list-schema.json
slug: x-api-list
source_filename: x-api-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-list-schema.json\",\n  \"title\": \"List\",\n  \"description\": \"A X List is a curated group of accounts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"follower_count\": {\n      \"type\": \"integer\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of this List.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"1146654567674912769\"\n    },\n    \"member_count\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of this List.\"\n    },\n    \"owner_id\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Unique identifier of this User. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"2244994945\"\n    },\n    \"private\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-list-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: List
---
