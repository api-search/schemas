---
description: Request body for updating a user
layout: schema
name: UserUpdateRequest
properties_list:
- description: ''
  name: data
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-user-update-request-schema.json
slug: prime-api-user-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-user-update-request-schema.json\",\n  \"title\": \"UserUpdateRequest\",\n  \"description\": \"Request body for updating a user\",\n  \"type\": \"object\",\n  \"required\": [\n    \"data\"\n  ],\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"id\",\n        \"type\",\n        \"attributes\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"User ID\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"user\"\n        },\n        \"attributes\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Updated user name\"\n            },\n\
  \            \"email\": {\n              \"type\": \"string\",\n              \"format\": \"email\",\n              \"description\": \"Updated email address\"\n            },\n            \"profile\": {\n              \"type\": \"string\",\n              \"description\": \"Updated profile bio\"\n            },\n            \"state\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"ACTIVE\",\n                \"DELETED\",\n                \"SUSPENDED\"\n              ]\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-user-update-request-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: UserUpdateRequest
---
