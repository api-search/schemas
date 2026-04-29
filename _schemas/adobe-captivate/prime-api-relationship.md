---
description: A JSON:API relationship object
layout: schema
name: Relationship
properties_list:
- description: ''
  name: data
  type: object
- description: ''
  name: links
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-relationship-schema.json
slug: prime-api-relationship
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-relationship-schema.json\",\n  \"title\": \"Relationship\",\n  \"description\": \"A JSON:API relationship object\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"oneOf\": [\n        {\n          \"type\": \"object\",\n          \"description\": \"JSON:API resource identifier\",\n          \"required\": [\n            \"id\",\n            \"type\"\n          ],\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"description\": \"Resource identifier\"\n            },\n            \"type\": {\n              \"type\": \"string\",\n              \"description\": \"Resource type name\"\n            }\n          }\n        },\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\
  ,\n            \"description\": \"JSON:API resource identifier\",\n            \"required\": [\n              \"id\",\n              \"type\"\n            ],\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"description\": \"Resource identifier\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"Resource type name\"\n              }\n            }\n          }\n        }\n      ]\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"related\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to fetch the related resource\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-relationship-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: Relationship
---
