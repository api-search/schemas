---
description: A GitHub organization.
layout: schema
name: organization-simple
properties_list:
- description: ''
  name: login
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: repos_url
  type: string
- description: ''
  name: events_url
  type: string
- description: ''
  name: hooks_url
  type: string
- description: ''
  name: issues_url
  type: string
- description: ''
  name: members_url
  type: string
- description: ''
  name: public_members_url
  type: string
- description: ''
  name: avatar_url
  type: string
- description: ''
  name: description
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-organizations-organization-simple-schema.json
slug: github-organizations-organization-simple
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-organizations-organization-simple-schema.json\",\n  \"title\": \"organization-simple\",\n  \"description\": \"A GitHub organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"login\": {\n      \"type\": \"string\",\n      \"example\": \"github\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDEyOk9yZ2FuaXphdGlvbjE=\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/orgs/github\"\n    },\n    \"repos_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/orgs/github/repos\"\n    },\n    \"events_url\": {\n      \"type\": \"string\",\n      \"format\": \"\
  uri\",\n      \"example\": \"https://api.github.com/orgs/github/events\"\n    },\n    \"hooks_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/orgs/github/hooks\"\n    },\n    \"issues_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/orgs/github/issues\"\n    },\n    \"members_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/orgs/github/members{/member}\"\n    },\n    \"public_members_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/orgs/github/public_members{/member}\"\n    },\n    \"avatar_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://github.com/images/error/octocat_happy.gif\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"A great organization\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"login\",\n    \"url\",\n    \"id\",\n    \"node_id\",\n    \"repos_url\",\n    \"events_url\"\
  ,\n    \"hooks_url\",\n    \"issues_url\",\n    \"members_url\",\n    \"public_members_url\",\n    \"avatar_url\",\n    \"description\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-organizations-organization-simple-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: organization-simple
---
