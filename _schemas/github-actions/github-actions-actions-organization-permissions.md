---
description: ''
layout: schema
name: ActionsOrganizationPermissions
properties_list:
- description: ''
  name: enabled_repositories
  type: string
- description: ''
  name: selected_repositories_url
  type: string
- description: ''
  name: allowed_actions
  type: string
- description: ''
  name: selected_actions_url
  type: string
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-actions-organization-permissions-schema.json
slug: github-actions-actions-organization-permissions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActionsOrganizationPermissions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled_repositories\": {\n      \"type\": \"string\"\n    },\n    \"selected_repositories_url\": {\n      \"type\": \"string\"\n    },\n    \"allowed_actions\": {\n      \"type\": \"string\"\n    },\n    \"selected_actions_url\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-actions-organization-permissions-schema.json
tags: []
title: ActionsOrganizationPermissions
---
