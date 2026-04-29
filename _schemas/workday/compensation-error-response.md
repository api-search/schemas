---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: error
  type: string
- description: ''
  name: errors
  type: array
provider_name: Workday
provider_slug: workday
schema_file: json-schema/compensation-error-response-schema.json
slug: compensation-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\"\n    },\n    \"errors\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/compensation-error-response-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: ErrorResponse
---
