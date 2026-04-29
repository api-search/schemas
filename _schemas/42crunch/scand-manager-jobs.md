---
description: Collection of all scan jobs
layout: schema
name: Jobs
properties_list:
- description: List of all scan job statuses
  name: jobs
  type: array
provider_name: 42Crunch
provider_slug: 42crunch
schema_file: json-schema/scand-manager-jobs-schema.json
slug: scand-manager-jobs
source_filename: scand-manager-jobs-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/42crunch/refs/heads/main/json-schema/scand-manager-jobs-schema.json\",\n  \"title\": \"Jobs\",\n  \"description\": \"Collection of all scan jobs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobs\": {\n      \"type\": \"array\",\n      \"description\": \"List of all scan job statuses\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobStatus\"\n      },\n      \"maxItems\": 1024,\n      \"example\": [\n        {\n          \"name\": \"scand-48340c78-a76c-475f-aa4a-36fc834b3c02\",\n          \"status\": \"active\"\n        }\n      ]\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/42crunch/refs/heads/main/json-schema/scand-manager-jobs-schema.json
tags:
- API Security
- Platform
- Scanning
- Security
- OpenAPI
- DevSecOps
title: Jobs
---
