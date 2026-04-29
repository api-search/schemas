---
description: Current status and result of an asynchronous job
layout: schema
name: JobStatus
properties_list:
- description: Unique identifier of the job
  name: jobId
  type: string
- description: Current job status
  name: status
  type: string
- description: ISO 8601 timestamp when the job was created
  name: created
  type: string
- description: ISO 8601 timestamp when the job was last modified
  name: modified
  type: string
- description: List of output files produced by a successful job
  name: outputs
  type: array
- description: List of errors if the job failed
  name: errors
  type: array
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-photoshop-job-status-schema.json
slug: adobe-creative-suite-photoshop-job-status
source_filename: adobe-creative-suite-photoshop-job-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-job-status-schema.json\",\n  \"title\": \"JobStatus\",\n  \"description\": \"Current status and result of an asynchronous job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the job\",\n      \"example\": \"f54e0fcb-260b-47c3-b520-de0d17dc2b67\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current job status\",\n      \"enum\": [\n        \"pending\",\n        \"running\",\n        \"succeeded\",\n        \"failed\"\n      ],\n      \"example\": \"succeeded\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the job was created\",\n      \"example\"\
  : \"example_value\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the job was last modified\",\n      \"example\": \"example_value\"\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"description\": \"List of output files produced by a successful job\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RenderOutput\"\n      }\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of errors if the job failed\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobError\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-job-status-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: JobStatus
---
