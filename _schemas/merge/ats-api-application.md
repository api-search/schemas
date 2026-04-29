---
description: An application linking a candidate to a job in the ATS.
layout: schema
name: Application
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: remote_id
  type: string
- description: ''
  name: candidate
  type: string
- description: ''
  name: job
  type: string
- description: ''
  name: applied_at
  type: string
- description: ''
  name: rejected_at
  type: string
- description: Candidate source channel.
  name: source
  type: string
- description: ''
  name: credited_to
  type: string
- description: ''
  name: current_stage
  type: string
- description: ''
  name: reject_reason
  type: string
- description: ''
  name: remote_was_deleted
  type: boolean
- description: ''
  name: created_at
  type: string
- description: ''
  name: modified_at
  type: string
provider_name: Merge
provider_slug: merge
schema_file: json-schema/ats-api-application-schema.json
slug: ats-api-application
source_filename: ats-api-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/json-schema/ats-api-application-schema.json\",\n  \"title\": \"Application\",\n  \"description\": \"An application linking a candidate to a job in the ATS.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"remote_id\": { \"type\": \"string\" },\n    \"candidate\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"job\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"applied_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"rejected_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"source\": { \"type\": \"string\", \"description\": \"Candidate source channel.\" },\n    \"credited_to\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"current_stage\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"reject_reason\"\
  : { \"type\": \"string\", \"format\": \"uuid\" },\n    \"remote_was_deleted\": { \"type\": \"boolean\" },\n    \"created_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"modified_at\": { \"type\": \"string\", \"format\": \"date-time\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/json-schema/ats-api-application-schema.json
tags:
- Integrations
- Platform
- Unified API
title: Application
---
