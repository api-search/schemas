---
description: Represents a single execution of a GitHub Actions workflow.
layout: schema
name: GitHub Actions Workflow Run
properties_list:
- description: The unique identifier of the workflow run.
  name: id
  type: integer
- description: The name of the workflow run.
  name: name
  type:
  - string
  - 'null'
- description: The GraphQL node ID of the workflow run.
  name: node_id
  type: string
- description: The branch associated with the workflow run's head commit.
  name: head_branch
  type:
  - string
  - 'null'
- description: The SHA of the head commit that points to the version of the workflow being run.
  name: head_sha
  type: string
- description: The path of the workflow file.
  name: path
  type: string
- description: The title of the workflow run as displayed in the GitHub UI.
  name: display_title
  type: string
- description: The auto-incrementing run number for the workflow run.
  name: run_number
  type: integer
- description: Attempt number of the run. 1 for the first attempt and higher if the workflow was re-run.
  name: run_attempt
  type: integer
- description: The event that triggered the workflow run.
  name: event
  type: string
- description: The current status of the workflow run.
  name: status
  type:
  - string
  - 'null'
- description: The result of the completed workflow run.
  name: conclusion
  type:
  - string
  - 'null'
- description: The ID of the parent workflow.
  name: workflow_id
  type: integer
- description: The API URL of the workflow run.
  name: url
  type: string
- description: The HTML URL of the workflow run on GitHub.
  name: html_url
  type: string
- description: The date and time the workflow run was created.
  name: created_at
  type: string
- description: The date and time the workflow run was last updated.
  name: updated_at
  type: string
- description: The date and time the workflow run started executing.
  name: run_started_at
  type: string
- description: The API URL for the jobs in this workflow run.
  name: jobs_url
  type: string
- description: The API URL for the logs of this workflow run.
  name: logs_url
  type: string
- description: The API URL for the artifacts of this workflow run.
  name: artifacts_url
  type: string
- description: The API URL to cancel this workflow run.
  name: cancel_url
  type: string
- description: The API URL to re-run this workflow run.
  name: rerun_url
  type: string
- description: The API URL of the parent workflow.
  name: workflow_url
  type: string
- description: The user who triggered the workflow run.
  name: actor
  type: object
- description: The user who triggered the workflow run (may differ from actor for re-runs).
  name: triggering_actor
  type: object
- description: The head commit for the workflow run.
  name: head_commit
  type:
  - object
  - 'null'
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-run-schema.json
slug: github-actions-run
source_filename: github-actions-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.github.com/actions/workflow-run.json\",\n  \"title\": \"GitHub Actions Workflow Run\",\n  \"description\": \"Represents a single execution of a GitHub Actions workflow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the workflow run.\"\n    },\n    \"name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The name of the workflow run.\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL node ID of the workflow run.\"\n    },\n    \"head_branch\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The branch associated with the workflow run's head commit.\"\n    },\n    \"head_sha\": {\n      \"type\": \"string\",\n      \"description\": \"The SHA of the head commit that points to the version of the workflow\
  \ being run.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The path of the workflow file.\"\n    },\n    \"display_title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the workflow run as displayed in the GitHub UI.\"\n    },\n    \"run_number\": {\n      \"type\": \"integer\",\n      \"description\": \"The auto-incrementing run number for the workflow run.\"\n    },\n    \"run_attempt\": {\n      \"type\": \"integer\",\n      \"description\": \"Attempt number of the run. 1 for the first attempt and higher if the workflow was re-run.\",\n      \"minimum\": 1\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"The event that triggered the workflow run.\",\n      \"examples\": [\"push\", \"pull_request\", \"workflow_dispatch\", \"schedule\", \"release\"]\n    },\n    \"status\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The current status of the workflow run.\",\n      \"\
  enum\": [\"queued\", \"in_progress\", \"completed\", \"waiting\", \"requested\", \"pending\", null]\n    },\n    \"conclusion\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The result of the completed workflow run.\",\n      \"enum\": [\"success\", \"failure\", \"neutral\", \"cancelled\", \"skipped\", \"timed_out\", \"action_required\", \"stale\", null]\n    },\n    \"workflow_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the parent workflow.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL of the workflow run.\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The HTML URL of the workflow run on GitHub.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the workflow run was created.\"\n    },\n    \"updated_at\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the workflow run was last updated.\"\n    },\n    \"run_started_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the workflow run started executing.\"\n    },\n    \"jobs_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL for the jobs in this workflow run.\"\n    },\n    \"logs_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL for the logs of this workflow run.\"\n    },\n    \"artifacts_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL for the artifacts of this workflow run.\"\n    },\n    \"cancel_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL to cancel this workflow run.\"\n    },\n    \"rerun_url\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL to re-run this workflow run.\"\n    },\n    \"workflow_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL of the parent workflow.\"\n    },\n    \"actor\": {\n      \"$ref\": \"github-actions-simple-user-schema.json\",\n      \"description\": \"The user who triggered the workflow run.\"\n    },\n    \"triggering_actor\": {\n      \"$ref\": \"github-actions-simple-user-schema.json\",\n      \"description\": \"The user who triggered the workflow run (may differ from actor for re-runs).\"\n    },\n    \"head_commit\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The head commit for the workflow run.\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"tree_id\": { \"type\": \"string\" },\n        \"message\": { \"type\": \"string\" },\n        \"timestamp\": { \"type\": \"string\", \"format\"\
  : \"date-time\" },\n        \"author\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": { \"type\": \"string\" },\n            \"email\": { \"type\": \"string\", \"format\": \"email\" }\n          }\n        },\n        \"committer\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": { \"type\": \"string\" },\n            \"email\": { \"type\": \"string\", \"format\": \"email\" }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"node_id\", \"head_sha\", \"run_number\", \"event\", \"status\", \"workflow_id\", \"url\", \"html_url\", \"created_at\", \"updated_at\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-run-schema.json
tags: []
title: GitHub Actions Workflow Run
---
