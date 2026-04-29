---
description: A reply to a discussion within a team.
layout: schema
name: team-discussion-comment
properties_list:
- description: ''
  name: author
  type: object
- description: The main text of the comment.
  name: body
  type: string
- description: ''
  name: body_html
  type: string
- description: The current version of the body content. If provided, this update operation will be rejected if the given version does not match the latest version on the server.
  name: body_version
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: last_edited_at
  type: string
- description: ''
  name: discussion_url
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: node_id
  type: string
- description: The unique sequence number of a team discussion comment.
  name: number
  type: integer
- description: ''
  name: updated_at
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: reactions
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-teams-team-discussion-comment-schema.json
slug: github-teams-team-discussion-comment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-teams-team-discussion-comment-schema.json\",\n  \"title\": \"team-discussion-comment\",\n  \"description\": \"A reply to a discussion within a team.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"author\": {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\n    },\n    \"body\": {\n      \"description\": \"The main text of the comment.\",\n      \"example\": \"I agree with this suggestion.\",\n      \"type\": \"string\"\n    },\n    \"body_html\": {\n      \"type\": \"string\",\n      \"example\": \"<p>Do you like apples?</p>\"\n    },\n    \"body_version\": {\n      \"description\": \"The current version of the body content. If provided, this update operation will be rejected if the given version does not match the latest version on the server.\",\n      \"example\": \"0307116bbf7ced493b8d8a346c650b71\"\
  ,\n      \"type\": \"string\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2018-01-15T23:53:58Z\"\n    },\n    \"last_edited_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"discussion_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/organizations/1/team/2403582/discussions/1\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/orgs/github/teams/justice-league/discussions/1/comments/1\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDIxOlRlYW1EaXNjdXNzaW9uQ29tbWVudDE=\"\n    },\n    \"number\": {\n      \"description\": \"The unique sequence number of a team discussion comment.\",\n      \"example\": 42,\n      \"type\": \"integer\"\n    },\n\
  \    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2018-01-15T23:53:58Z\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/organizations/1/team/2403582/discussions/1/comments/1\"\n    },\n    \"reactions\": {\n      \"$ref\": \"#/components/schemas/reaction-rollup\"\n    }\n  },\n  \"required\": [\n    \"author\",\n    \"body\",\n    \"body_html\",\n    \"body_version\",\n    \"created_at\",\n    \"last_edited_at\",\n    \"discussion_url\",\n    \"html_url\",\n    \"node_id\",\n    \"number\",\n    \"updated_at\",\n    \"url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-teams-team-discussion-comment-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: team-discussion-comment
---
