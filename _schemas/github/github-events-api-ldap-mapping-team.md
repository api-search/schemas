---
description: ldap-mapping-team from GitHub API
layout: schema
name: ldap-mapping-team
properties_list:
- description: ''
  name: ldap_dn
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
  name: html_url
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: slug
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: privacy
  type: string
- description: ''
  name: permission
  type: string
- description: ''
  name: members_url
  type: string
- description: ''
  name: repositories_url
  type: string
- description: ''
  name: parent
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-events-api-ldap-mapping-team-schema.json
slug: github-events-api-ldap-mapping-team
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-events-api-ldap-mapping-team-schema.json\",\n  \"title\": \"ldap-mapping-team\",\n  \"description\": \"ldap-mapping-team from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ldap_dn\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"12345678\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"octocat\"\n    },\n    \"slug\": {\n      \"\
  type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"This is an example repository\"\n    },\n    \"privacy\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"permission\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"members_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"repositories_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"parent\": {\n      \"nullable\": true,\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-events-api-ldap-mapping-team-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: ldap-mapping-team
---
