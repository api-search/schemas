---
description: ''
layout: schema
name: ActionsRepositoryPermissions
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: allowed_actions
  type: string
- description: ''
  name: selected_actions_url
  type: string
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-actions-repository-permissions-schema.json
slug: github-actions-actions-repository-permissions
source_filename: github-actions-actions-repository-permissions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActionsRepositoryPermissions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"allowed_actions\": {\n      \"type\": \"string\"\n    },\n    \"selected_actions_url\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-actions-repository-permissions-schema.json
tags: []
title: ActionsRepositoryPermissions
---
