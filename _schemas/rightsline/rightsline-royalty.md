---
description: A royalty or revenue record in the Rightsline platform
layout: schema
name: Rightsline Royalty
properties_list:
- description: Unique royalty record identifier
  name: id
  type: string
- description: Associated content identifier
  name: contentId
  type: string
- description: Revenue data type
  name: type
  type: string
- description: Royalty amount
  name: amount
  type: number
- description: Currency code (ISO 4217)
  name: currency
  type: string
- description: Reporting period
  name: period
  type: string
- description: Royalty record status
  name: status
  type: string
- description: Record creation timestamp
  name: createdAt
  type: string
provider_name: Rightsline
provider_slug: rightsline
schema_file: json-schema/rightsline-royalty-schema.json
slug: rightsline-royalty
source_filename: rightsline-royalty-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://github.com/api-evangelist/rightsline/blob/main/json-schema/rightsline-royalty-schema.json\",\n  \"title\": \"Rightsline Royalty\",\n  \"description\": \"A royalty or revenue record in the Rightsline platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique royalty record identifier\"\n    },\n    \"contentId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated content identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Revenue data type\",\n      \"enum\": [\"Revenue\", \"Sales\", \"Usage\"]\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Royalty amount\",\n      \"minimum\": 0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code (ISO 4217)\",\n   \
  \   \"example\": \"USD\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"period\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Reporting period\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Royalty record status\",\n      \"enum\": [\"Pending\", \"Approved\", \"Paid\"]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp\"\n    }\n  },\n  \"required\": [\"id\", \"contentId\", \"type\", \"amount\", \"currency\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/json-schema/rightsline-royalty-schema.json
tags:
- Content Management
- Entertainment
- Media
- Rights Management
- Royalties
title: Rightsline Royalty
---
