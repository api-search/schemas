---
description: ''
layout: schema
name: CampfireLine
properties_list:
- description: Line ID
  name: id
  type: integer
- description: Line status
  name: status
  type: string
- description: Timestamp when the line was posted
  name: created_at
  type: string
- description: Timestamp when the line was last updated
  name: updated_at
  type: string
- description: Line title (summary)
  name: title
  type: string
- description: Plain text message content
  name: content
  type: string
- description: Line type
  name: type
  type: string
- description: ''
  name: creator
  type: object
- description: ''
  name: bucket
  type: object
- description: ''
  name: parent
  type: object
- description: Number of boosts on this line
  name: boosts_count
  type: integer
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/campfireline-schema.json
slug: campfireline
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/campfireline-schema.json\",\n  \"title\": \"CampfireLine\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Line ID\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Line status\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the line was posted\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the line was last updated\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Line title (summary)\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Plain text message content\"\n    },\n    \"type\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Line type\"\n    },\n    \"creator\": {\n      \"$ref\": \"#/components/schemas/PersonRef\"\n    },\n    \"bucket\": {\n      \"$ref\": \"#/components/schemas/BucketRef\"\n    },\n    \"parent\": {\n      \"$ref\": \"#/components/schemas/Recording\"\n    },\n    \"boosts_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of boosts on this line\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/campfireline-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: CampfireLine
---
