---
description: Schema for CircleCI outbound webhook event payloads delivered via HTTP POST when workflow or job events occur in CI/CD pipelines.
layout: schema
name: CircleCI Webhook Event
properties_list:
- description: Unique identifier for the webhook delivery, used for deduplication
  name: id
  type: string
- description: The type of webhook event
  name: type
  type: string
- description: ISO 8601 timestamp of when the event occurred
  name: happened_at
  type: string
- description: ''
  name: webhook
  type: object
- description: ''
  name: project
  type: object
- description: ''
  name: organization
  type: object
- description: ''
  name: workflow
  type: object
- description: ''
  name: job
  type: object
- description: ''
  name: pipeline
  type: object
provider_name: CircleCI
provider_slug: circleci
schema_file: json-schema/circleci-webhook-event-schema.json
slug: circleci-webhook-event
tags:
- CI/CD
- Continuous Integration
- Continuous Deployment
- DevOps
- Pipelines
- Workflows
title: CircleCI Webhook Event
---
