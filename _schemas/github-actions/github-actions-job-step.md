---
description: ''
layout: schema
name: JobStep
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: conclusion
  type: string
- description: ''
  name: number
  type: integer
- description: ''
  name: started_at
  type: string
- description: ''
  name: completed_at
  type: string
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-job-step-schema.json
slug: github-actions-job-step
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobStep\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"conclusion\": {\n      \"type\": \"string\"\n    },\n    \"number\": {\n      \"type\": \"integer\"\n    },\n    \"started_at\": {\n      \"type\": \"string\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-job-step-schema.json
tags: []
title: JobStep
---
