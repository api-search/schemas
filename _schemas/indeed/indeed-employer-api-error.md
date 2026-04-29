---
description: An error returned by the Indeed API.
layout: schema
name: ApiError
properties_list:
- description: A machine-readable error code.
  name: code
  type: string
- description: A human-readable description of the error.
  name: message
  type: string
- description: The field that caused the error, if applicable.
  name: field
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-api-error-schema.json
slug: indeed-employer-api-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApiError\",\n  \"type\": \"object\",\n  \"description\": \"An error returned by the Indeed API.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"A machine-readable error code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the error.\"\n    },\n    \"field\": {\n      \"type\": \"string\",\n      \"description\": \"The field that caused the error, if applicable.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-api-error-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: ApiError
---
