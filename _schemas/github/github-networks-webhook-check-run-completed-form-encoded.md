---
description: The check_run.completed webhook encoded with URL encoding
layout: schema
name: webhook-check-run-completed-form-encoded
properties_list:
- description: A URL-encoded string of the check_run.completed JSON payload. The decoded payload is a JSON object.
  name: payload
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-networks-webhook-check-run-completed-form-encoded-schema.json
slug: github-networks-webhook-check-run-completed-form-encoded
source_filename: github-networks-webhook-check-run-completed-form-encoded-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-networks-webhook-check-run-completed-form-encoded-schema.json\",\n  \"title\": \"webhook-check-run-completed-form-encoded\",\n  \"description\": \"The check_run.completed webhook encoded with URL encoding\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"payload\": {\n      \"description\": \"A URL-encoded string of the check_run.completed JSON payload. The decoded payload is a JSON object.\",\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"payload\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-networks-webhook-check-run-completed-form-encoded-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: webhook-check-run-completed-form-encoded
---
