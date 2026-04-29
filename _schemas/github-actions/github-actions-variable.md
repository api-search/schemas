---
description: Represents a configuration variable for GitHub Actions workflows.
layout: schema
name: GitHub Actions Variable
properties_list:
- description: The name of the variable.
  name: name
  type: string
- description: The value of the variable.
  name: value
  type: string
- description: The date and time the variable was created.
  name: created_at
  type: string
- description: The date and time the variable was last updated.
  name: updated_at
  type: string
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-variable-schema.json
slug: github-actions-variable
source_filename: github-actions-variable-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.github.com/actions/variable.json\",\n  \"title\": \"GitHub Actions Variable\",\n  \"description\": \"Represents a configuration variable for GitHub Actions workflows.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the variable.\",\n      \"pattern\": \"^[A-Za-z_][A-Za-z0-9_]*$\",\n      \"examples\": [\"ENVIRONMENT\", \"DEPLOY_REGION\", \"NODE_VERSION\"]\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the variable.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the variable was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the variable was last updated.\"\n\
  \    }\n  },\n  \"required\": [\"name\", \"value\", \"created_at\", \"updated_at\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-variable-schema.json
tags: []
title: GitHub Actions Variable
---
