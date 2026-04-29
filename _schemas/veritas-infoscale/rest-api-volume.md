---
description: Volume schema from Veritas InfoScale REST API
layout: schema
name: Volume
properties_list:
- description: Volume name
  name: name
  type: string
- description: Parent disk group
  name: diskGroup
  type: string
- description: Volume state
  name: state
  type: string
- description: Volume size
  name: size
  type: string
- description: Volume layout type
  name: layout
  type: string
- description: Number of plexes
  name: plexCount
  type: integer
- description: Read policy for the volume
  name: readPolicy
  type: string
- description: Volume usage type
  name: usageType
  type: string
provider_name: Veritas InfoScale
provider_slug: veritas-infoscale
schema_file: json-schema/rest-api-volume-schema.json
slug: rest-api-volume
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/json-schema/rest-api-volume-schema.json\",\n  \"title\": \"Volume\",\n  \"description\": \"Volume schema from Veritas InfoScale REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Volume name\"\n    },\n    \"diskGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Parent disk group\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"ACTIVE\", \"DISABLED\", \"DETACHED\"],\n      \"description\": \"Volume state\"\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"Volume size\"\n    },\n    \"layout\": {\n      \"type\": \"string\",\n      \"enum\": [\"concat\", \"stripe\", \"mirror\", \"raid5\"],\n      \"description\": \"Volume layout type\"\n    },\n    \"plexCount\":\
  \ {\n      \"type\": \"integer\",\n      \"description\": \"Number of plexes\"\n    },\n    \"readPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"Read policy for the volume\"\n    },\n    \"usageType\": {\n      \"type\": \"string\",\n      \"description\": \"Volume usage type\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/json-schema/rest-api-volume-schema.json
tags:
- Clustering
- Data Management
- Disaster Recovery
- High Availability
- Storage Management
- Virtualization
title: Volume
---
