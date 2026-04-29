---
description: ''
layout: schema
name: WorkflowRun
properties_list:
- description: The ID of the workflow run.
  name: id
  type: integer
- description: The name of the workflow run.
  name: name
  type: string
- description: ''
  name: node_id
  type: string
- description: ''
  name: head_branch
  type: string
- description: The SHA of the head commit that points to the version of the workflow being run.
  name: head_sha
  type: string
- description: ''
  name: path
  type: string
- description: The title of the workflow run displayed in the UI.
  name: display_title
  type: string
- description: The auto incrementing run number for the workflow run.
  name: run_number
  type: integer
- description: Attempt number of the run, 1 for first attempt and higher if the workflow was re-run.
  name: run_attempt
  type: integer
- description: The event that triggered the workflow run.
  name: event
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: conclusion
  type: string
- description: ''
  name: workflow_id
  type: integer
- description: ''
  name: url
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: run_started_at
  type: string
- description: ''
  name: jobs_url
  type: string
- description: ''
  name: logs_url
  type: string
- description: ''
  name: artifacts_url
  type: string
- description: ''
  name: cancel_url
  type: string
- description: ''
  name: rerun_url
  type: string
- description: ''
  name: workflow_url
  type: string
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-workflow-run-schema.json
slug: github-actions-workflow-run
source_filename: github-actions-workflow-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkflowRun\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the workflow run.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workflow run.\"\n    },\n    \"node_id\": {\n      \"type\": \"string\"\n    },\n    \"head_branch\": {\n      \"type\": \"string\"\n    },\n    \"head_sha\": {\n      \"type\": \"string\",\n      \"description\": \"The SHA of the head commit that points to the version of the workflow being run.\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    },\n    \"display_title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the workflow run displayed in the UI.\"\n    },\n    \"run_number\": {\n      \"type\": \"integer\",\n      \"description\": \"The auto incrementing run number for the workflow run.\"\n    },\n\
  \    \"run_attempt\": {\n      \"type\": \"integer\",\n      \"description\": \"Attempt number of the run, 1 for first attempt and higher if the workflow was re-run.\"\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"The event that triggered the workflow run.\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"conclusion\": {\n      \"type\": \"string\"\n    },\n    \"workflow_id\": {\n      \"type\": \"integer\"\n    },\n    \"url\": {\n      \"type\": \"string\"\n    },\n    \"html_url\": {\n      \"type\": \"string\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    },\n    \"run_started_at\": {\n      \"type\": \"string\"\n    },\n    \"jobs_url\": {\n      \"type\": \"string\"\n    },\n    \"logs_url\": {\n      \"type\": \"string\"\n    },\n    \"artifacts_url\": {\n      \"type\": \"string\"\n    },\n    \"cancel_url\": {\n      \"type\": \"string\"\n    },\n\
  \    \"rerun_url\": {\n      \"type\": \"string\"\n    },\n    \"workflow_url\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-workflow-run-schema.json
tags: []
title: WorkflowRun
---
