---
description: collection of related issues and pull requests.
layout: schema
name: nullable-milestone
properties_list:
- description: ''
  name: url
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: labels_url
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: The number of the milestone.
  name: number
  type: integer
- description: The state of the milestone.
  name: state
  type: string
- description: The title of the milestone.
  name: title
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: creator
  type: object
- description: ''
  name: open_issues
  type: integer
- description: ''
  name: closed_issues
  type: integer
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: closed_at
  type: string
- description: ''
  name: due_on
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repo-pulls-api-nullable-milestone-schema.json
slug: github-repo-pulls-api-nullable-milestone
source_filename: github-repo-pulls-api-nullable-milestone-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-pulls-api-nullable-milestone-schema.json\",\n  \"title\": \"nullable-milestone\",\n  \"description\": \"collection of related issues and pull requests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World/milestones/1\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/octocat/Hello-World/milestones/v1.0\"\n    },\n    \"labels_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World/milestones/1/labels\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 1002604\n    },\n    \"node_id\"\
  : {\n      \"type\": \"string\",\n      \"example\": \"MDk6TWlsZXN0b25lMTAwMjYwNA==\"\n    },\n    \"number\": {\n      \"description\": \"The number of the milestone.\",\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"state\": {\n      \"description\": \"The state of the milestone.\",\n      \"example\": \"open\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"open\",\n        \"closed\"\n      ],\n      \"default\": \"open\"\n    },\n    \"title\": {\n      \"description\": \"The title of the milestone.\",\n      \"example\": \"v1.0\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Tracking milestone for version 1.0\"\n    },\n    \"creator\": {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\n    },\n    \"open_issues\": {\n      \"type\": \"integer\",\n      \"example\": 4\n    },\n    \"closed_issues\": {\n      \"type\": \"integer\",\n      \"example\": 8\n    },\n    \"\
  created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2011-04-10T20:09:31Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2014-03-03T18:58:10Z\"\n    },\n    \"closed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2013-02-12T13:22:01Z\"\n    },\n    \"due_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2012-10-09T23:39:01Z\"\n    }\n  },\n  \"required\": [\n    \"closed_issues\",\n    \"creator\",\n    \"description\",\n    \"due_on\",\n    \"closed_at\",\n    \"id\",\n    \"node_id\",\n    \"labels_url\",\n    \"html_url\",\n    \"number\",\n    \"open_issues\",\n    \"state\",\n    \"title\",\n    \"url\",\n    \"created_at\",\n    \"updated_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-pulls-api-nullable-milestone-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: nullable-milestone
---
