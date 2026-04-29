---
description: Current status and results of a Firefly generation job
layout: schema
name: GenerationStatus
properties_list:
- description: Unique identifier of the generation job
  name: jobId
  type: string
- description: Current status of the generation job
  name: status
  type: string
- description: ISO 8601 timestamp when the job was created
  name: created
  type: string
- description: ISO 8601 timestamp when the job was last modified
  name: modified
  type: string
- description: Generated output images or videos (present on success)
  name: outputs
  type: array
- description: Errors encountered during generation (present on failure)
  name: errors
  type: array
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-firefly-generation-status-schema.json
slug: adobe-creative-suite-firefly-generation-status
source_filename: adobe-creative-suite-firefly-generation-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-generation-status-schema.json\",\n  \"title\": \"GenerationStatus\",\n  \"description\": \"Current status and results of a Firefly generation job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the generation job\",\n      \"example\": \"urn:firefly:jobs:abc123def456\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the generation job\",\n      \"enum\": [\n        \"pending\",\n        \"running\",\n        \"succeeded\",\n        \"failed\"\n      ],\n      \"example\": \"succeeded\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when\
  \ the job was created\",\n      \"example\": \"example_value\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the job was last modified\",\n      \"example\": \"example_value\"\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"description\": \"Generated output images or videos (present on success)\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/OutputImage\"\n      }\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Errors encountered during generation (present on failure)\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"code\": {\n            \"type\": \"string\"\n          },\n          \"message\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-generation-status-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: GenerationStatus
---
