---
description: ListCreateRequest schema from X API v2
layout: schema
name: ListCreateRequest
properties_list:
- description: ''
  name: description
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: private
  type: boolean
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-list-create-request-schema.json
slug: x-api-list-create-request
source_filename: x-api-list-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-list-create-request-schema.json\",\n  \"title\": \"ListCreateRequest\",\n  \"description\": \"ListCreateRequest schema from X API v2\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"minLength\": 0,\n      \"maxLength\": 100\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"maxLength\": 25\n    },\n    \"private\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-list-create-request-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: ListCreateRequest
---
