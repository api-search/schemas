---
description: A group of users for organizing and targeting content
layout: schema
name: UserGroup
properties_list:
- description: Unique user group identifier
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
schema_file: json-schema/prime-api-user-group-schema.json
slug: prime-api-user-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-user-group-schema.json\",\n  \"title\": \"UserGroup\",\n  \"description\": \"A group of users for organizing and targeting content\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique user group identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"userGroup\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"dateCreated\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the group was created\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Group description\"\n        },\n        \"name\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Group name\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"Group state\",\n          \"enum\": [\n            \"Active\",\n            \"Deleted\"\n          ]\n        },\n        \"userCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of users in the group\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-user-group-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: UserGroup
---
