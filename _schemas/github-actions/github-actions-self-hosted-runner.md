---
description: ''
layout: schema
name: SelfHostedRunner
properties_list:
- description: The id of the runner.
  name: id
  type: integer
- description: The name of the runner.
  name: name
  type: string
- description: The operating system of the runner.
  name: os
  type: string
- description: The status of the runner.
  name: status
  type: string
- description: ''
  name: busy
  type: boolean
- description: ''
  name: labels
  type: array
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-self-hosted-runner-schema.json
slug: github-actions-self-hosted-runner
source_filename: github-actions-self-hosted-runner-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SelfHostedRunner\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The id of the runner.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the runner.\"\n    },\n    \"os\": {\n      \"type\": \"string\",\n      \"description\": \"The operating system of the runner.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the runner.\"\n    },\n    \"busy\": {\n      \"type\": \"boolean\"\n    },\n    \"labels\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-self-hosted-runner-schema.json
tags: []
title: SelfHostedRunner
---
