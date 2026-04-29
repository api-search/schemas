---
description: A team discussion is a persistent record of a free-form conversation within a team.
layout: schema
name: team-discussion
properties_list:
- description: ''
  name: author
  type: object
- description: The main text of the discussion.
  name: body
  type: string
- description: ''
  name: body_html
  type: string
- description: The current version of the body content. If provided, this update operation will be rejected if the given version does not match the latest version on the server.
  name: body_version
  type: string
- description: ''
  name: comments_count
  type: integer
- description: ''
  name: comments_url
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: last_edited_at
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: node_id
  type: string
- description: The unique sequence number of a team discussion.
  name: number
  type: integer
- description: Whether or not this discussion should be pinned for easy retrieval.
  name: pinned
  type: boolean
- description: Whether or not this discussion should be restricted to team members and organization owners.
  name: private
  type: boolean
- description: ''
  name: team_url
  type: string
- description: The title of the discussion.
  name: title
  type: string
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
schema_file: json-schema/github-teams-team-discussion-schema.json
slug: github-teams-team-discussion
source_filename: github-teams-team-discussion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-teams-team-discussion-schema.json\",\n  \"title\": \"team-discussion\",\n  \"description\": \"A team discussion is a persistent record of a free-form conversation within a team.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"author\": {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\n    },\n    \"body\": {\n      \"description\": \"The main text of the discussion.\",\n      \"example\": \"Please suggest improvements to our workflow in comments.\",\n      \"type\": \"string\"\n    },\n    \"body_html\": {\n      \"type\": \"string\",\n      \"example\": \"<p>Hi! This is an area for us to collaborate as a team</p>\"\n    },\n    \"body_version\": {\n      \"description\": \"The current version of the body content. If provided, this update operation will be rejected if the given version\
  \ does not match the latest version on the server.\",\n      \"example\": \"0307116bbf7ced493b8d8a346c650b71\",\n      \"type\": \"string\"\n    },\n    \"comments_count\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"comments_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/organizations/1/team/2343027/discussions/1/comments\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2018-01-25T18:56:31Z\"\n    },\n    \"last_edited_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/orgs/github/teams/justice-league/discussions/1\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDE0OlRlYW1EaXNjdXNzaW9uMQ==\"\
  \n    },\n    \"number\": {\n      \"description\": \"The unique sequence number of a team discussion.\",\n      \"example\": 42,\n      \"type\": \"integer\"\n    },\n    \"pinned\": {\n      \"description\": \"Whether or not this discussion should be pinned for easy retrieval.\",\n      \"example\": true,\n      \"type\": \"boolean\"\n    },\n    \"private\": {\n      \"description\": \"Whether or not this discussion should be restricted to team members and organization owners.\",\n      \"example\": true,\n      \"type\": \"boolean\"\n    },\n    \"team_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/organizations/1/team/2343027\"\n    },\n    \"title\": {\n      \"description\": \"The title of the discussion.\",\n      \"example\": \"How can we improve our workflow?\",\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2018-01-25T18:56:31Z\"\
  \n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/organizations/1/team/2343027/discussions/1\"\n    },\n    \"reactions\": {\n      \"$ref\": \"#/components/schemas/reaction-rollup\"\n    }\n  },\n  \"required\": [\n    \"author\",\n    \"body\",\n    \"body_html\",\n    \"body_version\",\n    \"comments_count\",\n    \"comments_url\",\n    \"created_at\",\n    \"last_edited_at\",\n    \"html_url\",\n    \"pinned\",\n    \"private\",\n    \"node_id\",\n    \"number\",\n    \"team_url\",\n    \"title\",\n    \"updated_at\",\n    \"url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-teams-team-discussion-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: team-discussion
---
