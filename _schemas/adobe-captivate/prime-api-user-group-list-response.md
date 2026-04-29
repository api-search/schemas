---
description: Paginated list of user groups
layout: schema
name: UserGroupListResponse
properties_list:
- description: ''
  name: data
  type: array
- description: Pagination links following JSON:API conventions
  name: links
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-user-group-list-response-schema.json
slug: prime-api-user-group-list-response
source_filename: prime-api-user-group-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-user-group-list-response-schema.json\",\n  \"title\": \"UserGroupListResponse\",\n  \"description\": \"Paginated list of user groups\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A group of users for organizing and targeting content\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique user group identifier\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"const\": \"userGroup\"\n          },\n          \"attributes\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"dateCreated\": {\n                \"type\": \"string\",\n\
  \                \"format\": \"date-time\",\n                \"description\": \"Timestamp when the group was created\"\n              },\n              \"description\": {\n                \"type\": \"string\",\n                \"description\": \"Group description\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Group name\"\n              },\n              \"state\": {\n                \"type\": \"string\",\n                \"description\": \"Group state\",\n                \"enum\": [\n                  \"Active\",\n                  \"Deleted\"\n                ]\n              },\n              \"userCount\": {\n                \"type\": \"integer\",\n                \"description\": \"Number of users in the group\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination links following JSON:API conventions\",\n\
  \      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the current page\"\n        },\n        \"next\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the next page\"\n        },\n        \"prev\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the previous page\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-user-group-list-response-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: UserGroupListResponse
---
