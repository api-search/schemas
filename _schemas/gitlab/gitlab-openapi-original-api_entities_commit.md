---
description: API_Entities_Commit from GitLab API
layout: schema
name: API_Entities_Commit
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: short_id
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: parent_ids
  type: array
- description: ''
  name: title
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: author_name
  type: string
- description: ''
  name: author_email
  type: string
- description: ''
  name: authored_date
  type: string
- description: ''
  name: committer_name
  type: string
- description: ''
  name: committer_email
  type: string
- description: ''
  name: committed_date
  type: string
- description: ''
  name: trailers
  type: object
- description: ''
  name: web_url
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-openapi-original-api_entities_commit-schema.json
slug: gitlab-openapi-original-api_entities_commit
source_filename: gitlab-openapi-original-api_entities_commit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-openapi-original-api_entities_commit-schema.json\",\n  \"title\": \"API_Entities_Commit\",\n  \"description\": \"API_Entities_Commit from GitLab API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"2695effb5807a22ff3d138d593fd856244e155e7\"\n    },\n    \"short_id\": {\n      \"type\": \"string\",\n      \"example\": \"2695effb\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2017-07-26 09:08:53+00:00\"\n    },\n    \"parent_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"example\": \"2a4b78934375d7f53875269ffd4f45fd83a84ebe\"\n      }\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"example\": \"Initial commit\"\
  \n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"Initial commit\"\n    },\n    \"author_name\": {\n      \"type\": \"string\",\n      \"example\": \"John Smith\"\n    },\n    \"author_email\": {\n      \"type\": \"string\",\n      \"example\": \"john@example.com\"\n    },\n    \"authored_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2012-05-28 11:42:42+00:00\"\n    },\n    \"committer_name\": {\n      \"type\": \"string\",\n      \"example\": \"Jack Smith\"\n    },\n    \"committer_email\": {\n      \"type\": \"string\",\n      \"example\": \"jack@example.com\"\n    },\n    \"committed_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2012-05-28 11:42:42+00:00\"\n    },\n    \"trailers\": {\n      \"type\": \"object\",\n      \"properties\": {},\n      \"example\": \"{ \\\"Merged-By\\\": \\\"Jane Doe janedoe@gitlab.com\\\" }\"\n    },\n    \"web_url\": {\n      \"\
  type\": \"string\",\n      \"example\": \"https://gitlab.example.com/janedoe/gitlab-foss/-/commit/ed899a2f4b50b4370feeea94676502b42383c746\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-openapi-original-api_entities_commit-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: API_Entities_Commit
---
