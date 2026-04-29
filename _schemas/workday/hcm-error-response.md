---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: A message describing the error.
  name: error
  type: string
- description: ''
  name: errors
  type: array
provider_name: Workday
provider_slug: workday
schema_file: json-schema/hcm-error-response-schema.json
slug: hcm-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"A message describing the error.\"\n    },\n    \"errors\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/hcm-error-response-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: ErrorResponse
---
