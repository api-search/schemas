---
description: A badge awarded to learners for achievements
layout: schema
name: Badge
properties_list:
- description: Unique badge identifier
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-badge-schema.json
slug: prime-api-badge
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-badge-schema.json\",\n  \"title\": \"Badge\",\n  \"description\": \"A badge awarded to learners for achievements\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique badge identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"badge\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"imageUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the badge image\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Badge name\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"Badge state\",\n          \"\
  enum\": [\n            \"Active\",\n            \"Retired\"\n          ]\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-badge-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: Badge
---
