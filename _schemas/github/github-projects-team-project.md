---
description: A team's access to a project.
layout: schema
name: team-project
properties_list:
- description: ''
  name: owner_url
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: columns_url
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: body
  type: string
- description: ''
  name: number
  type: integer
- description: ''
  name: state
  type: string
- description: ''
  name: creator
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: The organization permission for this project. Only present when owner is an organization.
  name: organization_permission
  type: string
- description: Whether the project is private or not. Only present when owner is an organization.
  name: private
  type: boolean
- description: ''
  name: permissions
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-projects-team-project-schema.json
slug: github-projects-team-project
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-projects-team-project-schema.json\",\n  \"title\": \"team-project\",\n  \"description\": \"A team's access to a project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"owner_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"columns_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"node_id\": {\n      \"type\": \"string\"\
  ,\n      \"example\": \"12345678\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"octocat\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"Example body text\"\n    },\n    \"number\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"example\": \"open\"\n    },\n    \"creator\": {\n      \"$ref\": \"#/components/schemas/simple-user\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"organization_permission\": {\n      \"description\": \"The organization permission for this project. Only present when owner is an organization.\",\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"private\": {\n      \"description\": \"Whether the project\
  \ is private or not. Only present when owner is an organization.\",\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"permissions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"read\": {\n          \"type\": \"boolean\"\n        },\n        \"write\": {\n          \"type\": \"boolean\"\n        },\n        \"admin\": {\n          \"type\": \"boolean\"\n        }\n      },\n      \"required\": [\n        \"read\",\n        \"write\",\n        \"admin\"\n      ]\n    }\n  },\n  \"required\": [\n    \"owner_url\",\n    \"url\",\n    \"html_url\",\n    \"columns_url\",\n    \"id\",\n    \"node_id\",\n    \"name\",\n    \"body\",\n    \"number\",\n    \"state\",\n    \"creator\",\n    \"created_at\",\n    \"updated_at\",\n    \"permissions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-projects-team-project-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: team-project
---
