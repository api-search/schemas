---
description: Webhook from GitLab API
layout: schema
name: Webhook
properties_list:
- description: The unique identifier of the webhook.
  name: id
  type: integer
- description: The URL that receives webhook POST requests.
  name: url
  type: string
- description: Optional name for the webhook.
  name: name
  type: string
- description: Optional description of the webhook.
  name: description
  type: string
- description: The ID of the project the webhook belongs to.
  name: project_id
  type: integer
- description: The date and time the webhook was created.
  name: created_at
  type: string
- description: Whether the webhook triggers on push events.
  name: push_events
  type: boolean
- description: Whether the webhook triggers on tag push events.
  name: tag_push_events
  type: boolean
- description: Whether the webhook triggers on issue events.
  name: issues_events
  type: boolean
- description: Whether the webhook triggers on confidential issue events.
  name: confidential_issues_events
  type: boolean
- description: Whether the webhook triggers on merge request events.
  name: merge_requests_events
  type: boolean
- description: Whether the webhook triggers on comment events.
  name: note_events
  type: boolean
- description: Whether the webhook triggers on confidential comment events.
  name: confidential_note_events
  type: boolean
- description: Whether the webhook triggers on job status change events.
  name: job_events
  type: boolean
- description: Whether the webhook triggers on pipeline status change events.
  name: pipeline_events
  type: boolean
- description: Whether the webhook triggers on wiki page events.
  name: wiki_page_events
  type: boolean
- description: Whether the webhook triggers on deployment events.
  name: deployment_events
  type: boolean
- description: Whether the webhook triggers on release events.
  name: releases_events
  type: boolean
- description: Whether the webhook triggers on group member events.
  name: member_events
  type: boolean
- description: Whether SSL certificate verification is enabled for the webhook URL.
  name: enable_ssl_verification
  type: boolean
- description: Branch name or wildcard pattern to filter push events.
  name: push_events_branch_filter
  type: string
- description: The strategy used for filtering branches.
  name: branch_filter_strategy
  type: string
- description: The current alert status of the webhook based on delivery failures.
  name: alert_status
  type: string
- description: If set, the webhook is temporarily disabled until this time.
  name: disabled_until
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-webhooks-webhook-schema.json
slug: gitlab-webhooks-webhook
source_filename: gitlab-webhooks-webhook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-webhooks-webhook-schema.json\",\n  \"title\": \"Webhook\",\n  \"description\": \"Webhook from GitLab API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the webhook.\",\n      \"example\": 42\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL that receives webhook POST requests.\",\n      \"example\": \"https://gitlab.com/example\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Optional name for the webhook.\",\n      \"example\": \"Example Project\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the webhook.\",\n      \"example\": \"Example description\"\
  \n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the project the webhook belongs to.\",\n      \"example\": 42\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the webhook was created.\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"push_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook triggers on push events.\",\n      \"example\": true\n    },\n    \"tag_push_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook triggers on tag push events.\",\n      \"example\": true\n    },\n    \"issues_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook triggers on issue events.\",\n      \"example\": true\n    },\n    \"confidential_issues_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook triggers on\
  \ confidential issue events.\",\n      \"example\": true\n    },\n    \"merge_requests_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook triggers on merge request events.\",\n      \"example\": true\n    },\n    \"note_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook triggers on comment events.\",\n      \"example\": true\n    },\n    \"confidential_note_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook triggers on confidential comment events.\",\n      \"example\": true\n    },\n    \"job_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook triggers on job status change events.\",\n      \"example\": true\n    },\n    \"pipeline_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook triggers on pipeline status change events.\",\n      \"example\": true\n    },\n    \"wiki_page_events\": {\n      \"type\"\
  : \"boolean\",\n      \"description\": \"Whether the webhook triggers on wiki page events.\",\n      \"example\": true\n    },\n    \"deployment_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook triggers on deployment events.\",\n      \"example\": true\n    },\n    \"releases_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook triggers on release events.\",\n      \"example\": true\n    },\n    \"member_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook triggers on group member events.\",\n      \"example\": true\n    },\n    \"enable_ssl_verification\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether SSL certificate verification is enabled for the webhook URL.\",\n      \"example\": true\n    },\n    \"push_events_branch_filter\": {\n      \"type\": \"string\",\n      \"description\": \"Branch name or wildcard pattern to filter push events.\",\n      \"example\"\
  : \"main\"\n    },\n    \"branch_filter_strategy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"wildcard\",\n        \"regex\",\n        \"all_branches\"\n      ],\n      \"description\": \"The strategy used for filtering branches.\",\n      \"example\": \"wildcard\"\n    },\n    \"alert_status\": {\n      \"type\": \"string\",\n      \"description\": \"The current alert status of the webhook based on delivery failures.\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"disabled_until\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"If set, the webhook is temporarily disabled until this time.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-webhooks-webhook-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: Webhook
---
