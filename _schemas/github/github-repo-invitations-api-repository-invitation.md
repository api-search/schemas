---
description: Repository invitations let you manage who you collaborate with.
layout: schema
name: repository-invitation
properties_list:
- description: Unique identifier of the repository invitation.
  name: id
  type: integer
- description: ''
  name: repository
  type: object
- description: ''
  name: invitee
  type: object
- description: ''
  name: inviter
  type: object
- description: The permission associated with the invitation.
  name: permissions
  type: string
- description: ''
  name: created_at
  type: string
- description: Whether or not the invitation has expired
  name: expired
  type: boolean
- description: URL for the repository invitation
  name: url
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: node_id
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repo-invitations-api-repository-invitation-schema.json
slug: github-repo-invitations-api-repository-invitation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-invitations-api-repository-invitation-schema.json\",\n  \"title\": \"repository-invitation\",\n  \"description\": \"Repository invitations let you manage who you collaborate with.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Unique identifier of the repository invitation.\",\n      \"example\": 42,\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"repository\": {\n      \"$ref\": \"#/components/schemas/minimal-repository\"\n    },\n    \"invitee\": {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\n    },\n    \"inviter\": {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\n    },\n    \"permissions\": {\n      \"description\": \"The permission associated with the invitation.\",\n      \"example\": \"read\"\
  ,\n      \"type\": \"string\",\n      \"enum\": [\n        \"read\",\n        \"write\",\n        \"admin\",\n        \"triage\",\n        \"maintain\"\n      ]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2016-06-13T14:52:50-05:00\"\n    },\n    \"expired\": {\n      \"description\": \"Whether or not the invitation has expired\",\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"url\": {\n      \"description\": \"URL for the repository invitation\",\n      \"example\": \"https://api.github.com/user/repository-invitations/1\",\n      \"type\": \"string\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://github.com/octocat/Hello-World/invitations\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"12345678\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"node_id\",\n    \"permissions\",\n    \"inviter\",\n    \"invitee\",\n  \
  \  \"repository\",\n    \"url\",\n    \"html_url\",\n    \"created_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-invitations-api-repository-invitation-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: repository-invitation
---
