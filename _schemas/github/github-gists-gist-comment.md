---
description: A comment made to a gist.
layout: schema
name: gist-comment
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: ''
  name: url
  type: string
- description: The comment text.
  name: body
  type: string
- description: ''
  name: user
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: author_association
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-gists-gist-comment-schema.json
slug: github-gists-gist-comment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-gists-gist-comment-schema.json\",\n  \"title\": \"gist-comment\",\n  \"description\": \"A comment made to a gist.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDExOkdpc3RDb21tZW50MQ==\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/gists/a6db0bec360bb87e9418/comments/1\"\n    },\n    \"body\": {\n      \"description\": \"The comment text.\",\n      \"type\": \"string\",\n      \"maxLength\": 65535,\n      \"example\": \"Body of the attachment\"\n    },\n    \"user\": {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\n    },\n    \"created_at\": {\n      \"type\":\
  \ \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2011-04-18T23:23:56Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2011-04-18T23:23:56Z\"\n    },\n    \"author_association\": {\n      \"$ref\": \"#/components/schemas/author-association\"\n    }\n  },\n  \"required\": [\n    \"url\",\n    \"id\",\n    \"node_id\",\n    \"user\",\n    \"body\",\n    \"author_association\",\n    \"created_at\",\n    \"updated_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-gists-gist-comment-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: gist-comment
---
