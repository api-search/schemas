---
description: ''
layout: schema
name: WorkflowRunUsage
properties_list:
- description: ''
  name: billable
  type: object
- description: ''
  name: run_duration_ms
  type: integer
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-workflow-run-usage-schema.json
slug: github-actions-workflow-run-usage
source_filename: github-actions-workflow-run-usage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkflowRunUsage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billable\": {\n      \"type\": \"object\"\n    },\n    \"run_duration_ms\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-workflow-run-usage-schema.json
tags: []
title: WorkflowRunUsage
---
