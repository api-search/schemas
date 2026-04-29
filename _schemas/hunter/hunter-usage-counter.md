---
description: ''
layout: schema
name: UsageCounter
properties_list:
- description: Number of requests used.
  name: used
  type: integer
- description: Number of requests available.
  name: available
  type: integer
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-usage-counter-schema.json
slug: hunter-usage-counter
source_filename: hunter-usage-counter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UsageCounter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"used\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of requests used.\"\n    },\n    \"available\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of requests available.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-usage-counter-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: UsageCounter
---
