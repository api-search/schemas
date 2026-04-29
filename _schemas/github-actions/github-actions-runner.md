---
description: Represents a self-hosted runner configured for GitHub Actions.
layout: schema
name: GitHub Actions Self-Hosted Runner
properties_list:
- description: The unique identifier of the runner.
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
- description: Whether the runner is currently executing a job.
  name: busy
  type: boolean
- description: Labels assigned to the runner.
  name: labels
  type: array
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-runner-schema.json
slug: github-actions-runner
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.github.com/actions/self-hosted-runner.json\",\n  \"title\": \"GitHub Actions Self-Hosted Runner\",\n  \"description\": \"Represents a self-hosted runner configured for GitHub Actions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the runner.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the runner.\",\n      \"examples\": [\"my-runner\", \"linux-build-01\"]\n    },\n    \"os\": {\n      \"type\": \"string\",\n      \"description\": \"The operating system of the runner.\",\n      \"examples\": [\"linux\", \"macos\", \"win\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the runner.\",\n      \"enum\": [\"online\", \"offline\"]\n    },\n    \"busy\": {\n      \"type\": \"boolean\",\n   \
  \   \"description\": \"Whether the runner is currently executing a job.\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels assigned to the runner.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"Unique identifier of the label.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the label.\",\n            \"examples\": [\"self-hosted\", \"linux\", \"x64\", \"gpu\"]\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The type of label.\",\n            \"enum\": [\"read-only\", \"custom\"]\n          }\n        },\n        \"required\": [\"id\", \"name\", \"type\"]\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\", \"os\", \"status\", \"busy\", \"labels\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-runner-schema.json
tags: []
title: GitHub Actions Self-Hosted Runner
---
