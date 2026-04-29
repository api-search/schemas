---
description: API_Entities_AccessRequester model
layout: schema
name: API_Entities_AccessRequester
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: username
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: avatar_url
  type: string
- description: ''
  name: avatar_path
  type: string
- description: ''
  name: custom_attributes
  type: array
- description: ''
  name: web_url
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: requested_at
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-api-v4-groups-api_entities_access-requester-schema.json
slug: gitlab-api-v4-groups-api_entities_access-requester
source_filename: gitlab-api-v4-groups-api_entities_access-requester-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-groups-api_entities_access-requester-schema.json\",\n  \"title\": \"API_Entities_AccessRequester\",\n  \"description\": \"API_Entities_AccessRequester model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 1\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"example\": \"admin\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Administrator\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"avatar_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://gravatar.com/avatar/1\"\n    },\n    \"avatar_path\": {\n      \"type\": \"string\",\n      \"example\": \"/user/avatar/28/The-Big-Lebowski-400-400.png\"\
  \n    },\n    \"custom_attributes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/API_Entities_CustomAttribute\"\n      }\n    },\n    \"web_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://gitlab.example.com/root\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"example\": \"user@example.com\"\n    },\n    \"requested_at\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-groups-api_entities_access-requester-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: API_Entities_AccessRequester
---
