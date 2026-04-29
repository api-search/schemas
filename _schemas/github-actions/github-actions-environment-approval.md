---
description: ''
layout: schema
name: EnvironmentApproval
properties_list:
- description: ''
  name: environments
  type: array
- description: ''
  name: state
  type: string
- description: ''
  name: comment
  type: string
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-environment-approval-schema.json
slug: github-actions-environment-approval
source_filename: github-actions-environment-approval-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvironmentApproval\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environments\": {\n      \"type\": \"array\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"comment\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-environment-approval-schema.json
tags: []
title: EnvironmentApproval
---
