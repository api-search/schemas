---
description: Request to install an integration on a target
layout: schema
name: integration-installation-request
properties_list:
- description: Unique identifier of the request installation.
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: ''
  name: account
  type: object
- description: ''
  name: requester
  type: object
- description: ''
  name: created_at
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-installation-integration-installation-request-schema.json
slug: github-installation-integration-installation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-installation-integration-installation-request-schema.json\",\n  \"title\": \"integration-installation-request\",\n  \"description\": \"Request to install an integration on a target\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Unique identifier of the request installation.\",\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDExOkludGVncmF0aW9uMQ==\"\n    },\n    \"account\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/simple-user\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/enterprise\"\n        }\n      ],\n      \"example\": \"example_value\"\n    },\n    \"requester\": {\n      \"$ref\": \"#/components/schemas/simple-user\"\
  \n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2022-07-08T16:18:44-04:00\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"account\",\n    \"requester\",\n    \"created_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-installation-integration-installation-request-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: integration-installation-request
---
