---
description: ''
layout: schema
name: PendingDeployment
properties_list:
- description: ''
  name: environment
  type: object
- description: ''
  name: wait_timer
  type: integer
- description: ''
  name: wait_timer_started_at
  type: string
- description: ''
  name: current_user_can_approve
  type: boolean
- description: ''
  name: reviewers
  type: array
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-pending-deployment-schema.json
slug: github-actions-pending-deployment
source_filename: github-actions-pending-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PendingDeployment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environment\": {\n      \"type\": \"object\"\n    },\n    \"wait_timer\": {\n      \"type\": \"integer\"\n    },\n    \"wait_timer_started_at\": {\n      \"type\": \"string\"\n    },\n    \"current_user_can_approve\": {\n      \"type\": \"boolean\"\n    },\n    \"reviewers\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-pending-deployment-schema.json
tags: []
title: PendingDeployment
---
