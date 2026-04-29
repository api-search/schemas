---
description: Groups of organization members that gives permissions on specified repositories.
layout: schema
name: team
properties_list:
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
  name: permissions
  type: object
- description: ''
  name: url
  type: string
- description: ''
  name: html_url
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
schema_file: json-schema/github-teams-team-schema.json
slug: github-teams-team
source_filename: github-teams-team-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-teams-team-schema.json\",\n  \"title\": \"team\",\n  \"description\": \"Groups of organization members that gives permissions on specified repositories.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"12345678\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"octocat\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"This is an example repository\"\n    },\n    \"privacy\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"permission\": {\n      \"\
  type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"permissions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"pull\": {\n          \"type\": \"boolean\"\n        },\n        \"triage\": {\n          \"type\": \"boolean\"\n        },\n        \"push\": {\n          \"type\": \"boolean\"\n        },\n        \"maintain\": {\n          \"type\": \"boolean\"\n        },\n        \"admin\": {\n          \"type\": \"boolean\"\n        }\n      },\n      \"required\": [\n        \"pull\",\n        \"triage\",\n        \"push\",\n        \"maintain\",\n        \"admin\"\n      ]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/orgs/rails/teams/core\"\n    },\n    \"members_url\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"repositories_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"parent\": {\n      \"$ref\": \"#/components/schemas/nullable-team-simple\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"node_id\",\n    \"url\",\n    \"members_url\",\n    \"name\",\n    \"description\",\n    \"permission\",\n    \"html_url\",\n    \"repositories_url\",\n    \"slug\",\n    \"parent\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-teams-team-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: team
---
