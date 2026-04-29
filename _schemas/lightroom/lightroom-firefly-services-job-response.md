---
description: ''
layout: schema
name: JobResponse
properties_list:
- description: Unique job identifier for tracking
  name: jobId
  type: string
- description: Job creation timestamp
  name: created
  type: string
- description: Job last modified timestamp
  name: modified
  type: string
- description: ''
  name: outputs
  type: array
- description: ''
  name: _links
  type: object
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-firefly-services-job-response-schema.json
slug: lightroom-firefly-services-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique job identifier for tracking\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"Job creation timestamp\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"description\": \"Job last modified timestamp\"\n    },\n    \"outputs\": {\n      \"type\": \"array\"\n    },\n    \"_links\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-firefly-services-job-response-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: JobResponse
---
