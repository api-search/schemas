---
description: ''
layout: schema
name: VerificationStatus
properties_list:
- description: Date the verification was performed.
  name: date
  type: '[''string'', ''null'']'
- description: The verification status.
  name: status
  type: '[''string'', ''null'']'
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-verification-status-schema.json
slug: hunter-verification-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VerificationStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Date the verification was performed.\"\n    },\n    \"status\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The verification status.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-verification-status-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: VerificationStatus
---
