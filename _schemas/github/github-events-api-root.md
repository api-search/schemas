---
description: root from GitHub API
layout: schema
name: root
properties_list:
- description: ''
  name: current_user_url
  type: string
- description: ''
  name: current_user_authorizations_html_url
  type: string
- description: ''
  name: authorizations_url
  type: string
- description: ''
  name: code_search_url
  type: string
- description: ''
  name: commit_search_url
  type: string
- description: ''
  name: emails_url
  type: string
- description: ''
  name: emojis_url
  type: string
- description: ''
  name: events_url
  type: string
- description: ''
  name: feeds_url
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
  name: hub_url
  type: string
- description: ''
  name: issue_search_url
  type: string
- description: ''
  name: issues_url
  type: string
- description: ''
  name: keys_url
  type: string
- description: ''
  name: label_search_url
  type: string
- description: ''
  name: notifications_url
  type: string
- description: ''
  name: organization_url
  type: string
- description: ''
  name: organization_repositories_url
  type: string
- description: ''
  name: organization_teams_url
  type: string
- description: ''
  name: public_gists_url
  type: string
- description: ''
  name: rate_limit_url
  type: string
- description: ''
  name: repository_url
  type: string
- description: ''
  name: repository_search_url
  type: string
- description: ''
  name: current_user_repositories_url
  type: string
- description: ''
  name: starred_url
  type: string
- description: ''
  name: starred_gists_url
  type: string
- description: ''
  name: topic_search_url
  type: string
- description: ''
  name: user_url
  type: string
- description: ''
  name: user_organizations_url
  type: string
- description: ''
  name: user_repositories_url
  type: string
- description: ''
  name: user_search_url
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-events-api-root-schema.json
slug: github-events-api-root
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-events-api-root-schema.json\",\n  \"title\": \"root\",\n  \"description\": \"root from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"current_user_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"current_user_authorizations_html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"authorizations_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"code_search_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\
  \n    },\n    \"commit_search_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"emails_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"emojis_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"events_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"feeds_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"followers_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\
  \n    },\n    \"following_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"gists_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"hub_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"deprecated\": true,\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"issue_search_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"issues_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"keys_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\":\
  \ \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"label_search_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"notifications_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"organization_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"organization_repositories_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"organization_teams_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\"\n    },\n    \"public_gists_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\"\n    },\n    \"rate_limit_url\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"uri-template\"\n    },\n    \"repository_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\"\n    },\n    \"repository_search_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\"\n    },\n    \"current_user_repositories_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\"\n    },\n    \"starred_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\"\n    },\n    \"starred_gists_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\"\n    },\n    \"topic_search_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\"\n    },\n    \"user_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\"\n    },\n    \"user_organizations_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\"\n    },\n    \"user_repositories_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\"\
  \n    },\n    \"user_search_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri-template\"\n    }\n  },\n  \"required\": [\n    \"current_user_url\",\n    \"current_user_authorizations_html_url\",\n    \"authorizations_url\",\n    \"code_search_url\",\n    \"commit_search_url\",\n    \"emails_url\",\n    \"emojis_url\",\n    \"events_url\",\n    \"feeds_url\",\n    \"followers_url\",\n    \"following_url\",\n    \"gists_url\",\n    \"issue_search_url\",\n    \"issues_url\",\n    \"keys_url\",\n    \"label_search_url\",\n    \"notifications_url\",\n    \"organization_url\",\n    \"organization_repositories_url\",\n    \"organization_teams_url\",\n    \"public_gists_url\",\n    \"rate_limit_url\",\n    \"repository_url\",\n    \"repository_search_url\",\n    \"current_user_repositories_url\",\n    \"starred_url\",\n    \"starred_gists_url\",\n    \"user_url\",\n    \"user_organizations_url\",\n    \"user_repositories_url\",\n    \"user_search_url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-events-api-root-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: root
---
