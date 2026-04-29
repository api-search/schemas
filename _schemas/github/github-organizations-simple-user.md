---
description: A GitHub user.
layout: schema
name: simple-user
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: email
  type: string
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
  name: avatar_url
  type: string
- description: ''
  name: gravatar_id
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: followers_url
  type: string
- description: ''
  name: following_url
  type: string
- description: ''
  name: gists_url
  type: string
- description: ''
  name: starred_url
  type: string
- description: ''
  name: subscriptions_url
  type: string
- description: ''
  name: organizations_url
  type: string
- description: ''
  name: repos_url
  type: string
- description: ''
  name: events_url
  type: string
- description: ''
  name: received_events_url
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: site_admin
  type: boolean
- description: ''
  name: starred_at
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-organizations-simple-user-schema.json
slug: github-organizations-simple-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-organizations-simple-user-schema.json\",\n  \"title\": \"simple-user\",\n  \"description\": \"A GitHub user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"nullable\": true,\n      \"type\": \"string\",\n      \"example\": \"octocat\"\n    },\n    \"email\": {\n      \"nullable\": true,\n      \"type\": \"string\",\n      \"example\": \"octocat@github.com\"\n    },\n    \"login\": {\n      \"type\": \"string\",\n      \"example\": \"octocat\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDQ6VXNlcjE=\"\n    },\n    \"avatar_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/images/error/octocat_happy.gif\"\n    },\n\
  \    \"gravatar_id\": {\n      \"type\": \"string\",\n      \"example\": \"41d064eb2195891e12d0413f63227ea7\",\n      \"nullable\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/users/octocat\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/octocat\"\n    },\n    \"followers_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/users/octocat/followers\"\n    },\n    \"following_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/users/octocat/following{/other_user}\"\n    },\n    \"gists_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/users/octocat/gists{/gist_id}\"\n    },\n    \"starred_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/users/octocat/starred{/owner}{/repo}\"\
  \n    },\n    \"subscriptions_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/users/octocat/subscriptions\"\n    },\n    \"organizations_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/users/octocat/orgs\"\n    },\n    \"repos_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/users/octocat/repos\"\n    },\n    \"events_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/users/octocat/events{/privacy}\"\n    },\n    \"received_events_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/users/octocat/received_events\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"User\"\n    },\n    \"site_admin\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"starred_at\": {\n\
  \      \"type\": \"string\",\n      \"example\": \"\\\"2020-07-09T00:17:55Z\\\"\"\n    }\n  },\n  \"required\": [\n    \"avatar_url\",\n    \"events_url\",\n    \"followers_url\",\n    \"following_url\",\n    \"gists_url\",\n    \"gravatar_id\",\n    \"html_url\",\n    \"id\",\n    \"node_id\",\n    \"login\",\n    \"organizations_url\",\n    \"received_events_url\",\n    \"repos_url\",\n    \"site_admin\",\n    \"starred_url\",\n    \"subscriptions_url\",\n    \"type\",\n    \"url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-organizations-simple-user-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: simple-user
---
