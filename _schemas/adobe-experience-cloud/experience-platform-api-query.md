---
description: Query schema
layout: schema
name: Query
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: dbName
  type: string
- description: ''
  name: sql
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: updated
  type: string
- description: ''
  name: rowCount
  type: integer
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/experience-platform-api-query-schema.json
slug: experience-platform-api-query
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-query-schema.json\",\n  \"title\": \"Query\",\n  \"description\": \"Query schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"dbName\": {\n      \"type\": \"string\"\n    },\n    \"sql\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SUBMITTED\",\n        \"IN_PROGRESS\",\n        \"SUCCESS\",\n        \"FAILED\"\n      ]\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"rowCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-query-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: Query
---
