---
description: Installation
layout: schema
name: installation
properties_list:
- description: The ID of the installation.
  name: id
  type: integer
- description: ''
  name: account
  type: object
- description: Describe whether all repositories have been selected or there's a selection involved
  name: repository_selection
  type: string
- description: ''
  name: access_tokens_url
  type: string
- description: ''
  name: repositories_url
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: app_id
  type: integer
- description: The ID of the user or organization this token is being scoped to.
  name: target_id
  type: integer
- description: ''
  name: target_type
  type: string
- description: ''
  name: permissions
  type: object
- description: ''
  name: events
  type: array
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: single_file_name
  type: string
- description: ''
  name: has_multiple_single_files
  type: boolean
- description: ''
  name: single_file_paths
  type: array
- description: ''
  name: app_slug
  type: string
- description: ''
  name: suspended_by
  type: object
- description: ''
  name: suspended_at
  type: string
- description: ''
  name: contact_email
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-installation-installation-schema.json
slug: github-installation-installation
source_filename: github-installation-installation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-installation-installation-schema.json\",\n  \"title\": \"installation\",\n  \"description\": \"Installation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"The ID of the installation.\",\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"account\": {\n      \"nullable\": true,\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/simple-user\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/enterprise\"\n        }\n      ],\n      \"example\": \"example_value\"\n    },\n    \"repository_selection\": {\n      \"description\": \"Describe whether all repositories have been selected or there's a selection involved\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"all\",\n        \"selected\"\n      ],\n\
  \      \"example\": \"all\"\n    },\n    \"access_tokens_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/app/installations/1/access_tokens\"\n    },\n    \"repositories_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/installation/repositories\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/organizations/github/settings/installations/1\"\n    },\n    \"app_id\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"target_id\": {\n      \"description\": \"The ID of the user or organization this token is being scoped to.\",\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"target_type\": {\n      \"type\": \"string\",\n      \"example\": \"Organization\"\n    },\n    \"permissions\": {\n      \"$ref\": \"#/components/schemas/app-permissions\"\n    },\n\
  \    \"events\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"single_file_name\": {\n      \"type\": \"string\",\n      \"example\": \"config.yaml\",\n      \"nullable\": true\n    },\n    \"has_multiple_single_files\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"single_file_paths\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"config.yml\",\n        \".github/issue_TEMPLATE.md\"\n      ]\n    },\n    \"app_slug\": {\n      \"type\": \"string\",\n      \"example\": \"github-actions\"\n    },\n    \"suspended_by\": {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\
  \n    },\n    \"suspended_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"contact_email\": {\n      \"type\": \"string\",\n      \"example\": \"\\\"test_13f1e99741e3e004@d7e1eb0bc0a1ba12.com\\\"\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"app_id\",\n    \"app_slug\",\n    \"target_id\",\n    \"target_type\",\n    \"single_file_name\",\n    \"repository_selection\",\n    \"access_tokens_url\",\n    \"html_url\",\n    \"repositories_url\",\n    \"events\",\n    \"account\",\n    \"permissions\",\n    \"created_at\",\n    \"updated_at\",\n    \"suspended_by\",\n    \"suspended_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-installation-installation-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: installation
---
