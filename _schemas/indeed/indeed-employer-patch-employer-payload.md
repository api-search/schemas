---
description: Response payload from a successful employer create or update operation.
layout: schema
name: PatchEmployerPayload
properties_list:
- description: Whether the operation succeeded.
  name: success
  type: boolean
- description: Any errors encountered during the operation.
  name: errors
  type: array
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-patch-employer-payload-schema.json
slug: indeed-employer-patch-employer-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PatchEmployerPayload\",\n  \"type\": \"object\",\n  \"description\": \"Response payload from a successful employer create or update operation.\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the operation succeeded.\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Any errors encountered during the operation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-patch-employer-payload-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: PatchEmployerPayload
---
