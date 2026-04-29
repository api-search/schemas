---
description: WebhookInput from GitLab API
layout: schema
name: WebhookInput
properties_list:
- description: The URL to send webhook POST requests to.
  name: url
  type: string
- description: Optional name for the webhook.
  name: name
  type: string
- description: Optional description of the webhook.
  name: description
  type: string
- description: A secret token to validate received payloads. Sent as the X-Gitlab-Token header.
  name: secret_token
  type: string
- description: Whether to verify SSL certificates on the webhook URL.
  name: enable_ssl_verification
  type: boolean
- description: Trigger on push events.
  name: push_events
  type: boolean
- description: Trigger on tag push events.
  name: tag_push_events
  type: boolean
- description: Trigger on issue events.
  name: issues_events
  type: boolean
- description: Trigger on confidential issue events.
  name: confidential_issues_events
  type: boolean
- description: Trigger on merge request events.
  name: merge_requests_events
  type: boolean
- description: Trigger on comment events.
  name: note_events
  type: boolean
- description: Trigger on confidential comment events.
  name: confidential_note_events
  type: boolean
- description: Trigger on job status change events.
  name: job_events
  type: boolean
- description: Trigger on pipeline status change events.
  name: pipeline_events
  type: boolean
- description: Trigger on wiki page events.
  name: wiki_page_events
  type: boolean
- description: Trigger on deployment events.
  name: deployment_events
  type: boolean
- description: Trigger on release events.
  name: releases_events
  type: boolean
- description: Trigger on group member events.
  name: member_events
  type: boolean
- description: Branch name or wildcard pattern to filter push events.
  name: push_events_branch_filter
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-webhooks-webhook-input-schema.json
slug: gitlab-webhooks-webhook-input
source_filename: gitlab-webhooks-webhook-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-webhooks-webhook-input-schema.json\",\n  \"title\": \"WebhookInput\",\n  \"description\": \"WebhookInput from GitLab API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to send webhook POST requests to.\",\n      \"example\": \"https://gitlab.com/example\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Optional name for the webhook.\",\n      \"example\": \"Example Project\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the webhook.\",\n      \"example\": \"Example description\"\n    },\n    \"secret_token\": {\n      \"type\": \"string\",\n      \"description\": \"A secret token to validate received payloads.\
  \ Sent as the X-Gitlab-Token header.\",\n      \"example\": \"glpat-example-token\"\n    },\n    \"enable_ssl_verification\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to verify SSL certificates on the webhook URL.\",\n      \"example\": true\n    },\n    \"push_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on push events.\",\n      \"example\": true\n    },\n    \"tag_push_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on tag push events.\",\n      \"example\": true\n    },\n    \"issues_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on issue events.\",\n      \"example\": true\n    },\n    \"confidential_issues_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on confidential issue events.\",\n      \"example\": true\n    },\n    \"merge_requests_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on merge request events.\"\
  ,\n      \"example\": true\n    },\n    \"note_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on comment events.\",\n      \"example\": true\n    },\n    \"confidential_note_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on confidential comment events.\",\n      \"example\": true\n    },\n    \"job_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on job status change events.\",\n      \"example\": true\n    },\n    \"pipeline_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on pipeline status change events.\",\n      \"example\": true\n    },\n    \"wiki_page_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on wiki page events.\",\n      \"example\": true\n    },\n    \"deployment_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on deployment events.\",\n      \"example\": true\n    },\n    \"releases_events\": {\n      \"\
  type\": \"boolean\",\n      \"description\": \"Trigger on release events.\",\n      \"example\": true\n    },\n    \"member_events\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on group member events.\",\n      \"example\": true\n    },\n    \"push_events_branch_filter\": {\n      \"type\": \"string\",\n      \"description\": \"Branch name or wildcard pattern to filter push events.\",\n      \"example\": \"main\"\n    }\n  },\n  \"required\": [\n    \"url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-webhooks-webhook-input-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: WebhookInput
---
