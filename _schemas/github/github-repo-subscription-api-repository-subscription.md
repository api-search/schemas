---
description: Repository invitations let you manage who you collaborate with.
layout: schema
name: repository-subscription
properties_list:
- description: Determines if notifications should be received from this repository.
  name: subscribed
  type: boolean
- description: Determines if all notifications should be blocked from this repository.
  name: ignored
  type: boolean
- description: ''
  name: reason
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: repository_url
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repo-subscription-api-repository-subscription-schema.json
slug: github-repo-subscription-api-repository-subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-subscription-api-repository-subscription-schema.json\",\n  \"title\": \"repository-subscription\",\n  \"description\": \"Repository invitations let you manage who you collaborate with.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subscribed\": {\n      \"description\": \"Determines if notifications should be received from this repository.\",\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"ignored\": {\n      \"description\": \"Determines if all notifications should be blocked from this repository.\",\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2012-10-06T21:34:12Z\"\
  \n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/example/subscription\"\n    },\n    \"repository_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/example\"\n    }\n  },\n  \"required\": [\n    \"created_at\",\n    \"ignored\",\n    \"reason\",\n    \"subscribed\",\n    \"url\",\n    \"repository_url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-subscription-api-repository-subscription-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: repository-subscription
---
