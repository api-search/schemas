---
description: Current status of a conformance scan job
layout: schema
name: JobStatus
properties_list:
- description: ''
  name: name
  type: object
- description: Current lifecycle status of the job
  name: status
  type: string
provider_name: 42Crunch
provider_slug: 42crunch
schema_file: json-schema/scand-manager-job-status-schema.json
slug: scand-manager-job-status
source_filename: scand-manager-job-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/42crunch/refs/heads/main/json-schema/scand-manager-job-status-schema.json\",\n  \"title\": \"JobStatus\",\n  \"description\": \"Current status of a conformance scan job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"$ref\": \"#/components/schemas/JobName\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the job\",\n      \"enum\": [\n        \"started\",\n        \"active\",\n        \"succeeded\",\n        \"failed\",\n        \"unknown\",\n        \"deleted\"\n      ],\n      \"example\": \"active\"\n    }\n  },\n  \"additionalProperties\": false,\n  \"required\": [\n    \"name\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/42crunch/refs/heads/main/json-schema/scand-manager-job-status-schema.json
tags:
- API Security
- Platform
- Scanning
- Security
- OpenAPI
- DevSecOps
title: JobStatus
---
