---
description: ''
layout: schema
name: LeadsList
properties_list:
- description: Unique identifier for the leads list.
  name: id
  type: integer
- description: Name of the leads list.
  name: name
  type: string
- description: Number of leads in the list.
  name: leads_count
  type: integer
- description: Timestamp when the list was created.
  name: created_at
  type: string
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-leads-list-schema.json
slug: hunter-leads-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LeadsList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the leads list.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the leads list.\"\n    },\n    \"leads_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of leads in the list.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the list was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-leads-list-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: LeadsList
---
