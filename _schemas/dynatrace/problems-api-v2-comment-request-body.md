---
description: The request body for creating or updating a problem comment.
layout: schema
name: CommentRequestBody
properties_list:
- description: The text content of the comment.
  name: message
  type: string
- description: An optional context reference for the comment, such as a ticket ID, a link to a runbook, or a category label.
  name: context
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/problems-api-v2-comment-request-body-schema.json
slug: problems-api-v2-comment-request-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-api-v2-comment-request-body-schema.json\",\n  \"title\": \"CommentRequestBody\",\n  \"description\": \"The request body for creating or updating a problem comment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The text content of the comment.\",\n      \"example\": \"Example description.\"\n    },\n    \"context\": {\n      \"type\": \"string\",\n      \"description\": \"An optional context reference for the comment, such as a ticket ID, a link to a runbook, or a category label.\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"required\": [\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-api-v2-comment-request-body-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: CommentRequestBody
---
