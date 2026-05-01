---
description: Request body for creating a job queue.
layout: schema
name: Create Queue Request
properties_list:
- description: ''
  name: displayName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: defaultBudgetAction
  type: string
provider_name: Amazon Deadline Cloud
provider_slug: amazon-deadline-cloud
schema_file: json-schema/create-queue-request-schema.json
slug: create-queue-request
source_filename: create-queue-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deadline-cloud/json-schema/create-queue-request-schema.json\",\n  \"title\": \"Create Queue Request\",\n  \"description\": \"Request body for creating a job queue.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"displayName\"\n  ],\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"defaultBudgetAction\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/json-schema/create-queue-request-schema.json
tags:
- Compute
- Media
- Rendering
- Visual Effects
title: Create Queue Request
---
