---
description: Paginated list of badges
layout: schema
name: BadgeListResponse
properties_list:
- description: ''
  name: data
  type: array
- description: Pagination links following JSON:API conventions
  name: links
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-badge-list-response-schema.json
slug: prime-api-badge-list-response
source_filename: prime-api-badge-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-badge-list-response-schema.json\",\n  \"title\": \"BadgeListResponse\",\n  \"description\": \"Paginated list of badges\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A badge awarded to learners for achievements\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique badge identifier\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"const\": \"badge\"\n          },\n          \"attributes\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"imageUrl\": {\n                \"type\": \"string\",\n                \"format\": \"uri\"\
  ,\n                \"description\": \"URL of the badge image\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Badge name\"\n              },\n              \"state\": {\n                \"type\": \"string\",\n                \"description\": \"Badge state\",\n                \"enum\": [\n                  \"Active\",\n                  \"Retired\"\n                ]\n              }\n            }\n          }\n        }\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination links following JSON:API conventions\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the current page\"\n        },\n        \"next\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the next page\"\n        },\n        \"prev\": {\n      \
  \    \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the previous page\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-badge-list-response-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: BadgeListResponse
---
