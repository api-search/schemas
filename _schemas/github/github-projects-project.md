---
description: Projects are a way to organize columns and cards of work.
layout: schema
name: project
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
- description: Name of the project
  name: name
  type: string
- description: Body of the project
  name: body
  type: string
- description: ''
  name: number
  type: integer
- description: State of the project; either 'open' or 'closed'
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
- description: The baseline permission that all organization members have on this project. Only present if owner is an organization.
  name: organization_permission
  type: string
- description: Whether or not this project can be seen by everyone. Only present if owner is an organization.
  name: private
  type: boolean
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-projects-project-schema.json
slug: github-projects-project
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-projects-project-schema.json\",\n  \"title\": \"project\",\n  \"description\": \"Projects are a way to organize columns and cards of work.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"owner_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/api-playground/projects-test\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/projects/1002604\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/api-playground/projects-test/projects/12\"\n    },\n    \"columns_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/projects/1002604/columns\"\
  \n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 1002604\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDc6UHJvamVjdDEwMDI2MDQ=\"\n    },\n    \"name\": {\n      \"description\": \"Name of the project\",\n      \"example\": \"Week One Sprint\",\n      \"type\": \"string\"\n    },\n    \"body\": {\n      \"description\": \"Body of the project\",\n      \"example\": \"This project represents the sprint of the first week in January\",\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"number\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"state\": {\n      \"description\": \"State of the project; either 'open' or 'closed'\",\n      \"example\": \"open\",\n      \"type\": \"string\"\n    },\n    \"creator\": {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2011-04-10T20:09:31Z\"\
  \n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2014-03-03T18:58:10Z\"\n    },\n    \"organization_permission\": {\n      \"description\": \"The baseline permission that all organization members have on this project. Only present if owner is an organization.\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"read\",\n        \"write\",\n        \"admin\",\n        \"none\"\n      ],\n      \"example\": \"read\"\n    },\n    \"private\": {\n      \"description\": \"Whether or not this project can be seen by everyone. Only present if owner is an organization.\",\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"node_id\",\n    \"number\",\n    \"name\",\n    \"body\",\n    \"state\",\n    \"url\",\n    \"html_url\",\n    \"owner_url\",\n    \"creator\",\n    \"columns_url\",\n    \"created_at\",\n    \"updated_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-projects-project-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: project
---
