---
description: ''
layout: schema
name: DiscoverResult
properties_list:
- description: Domain name of the discovered company.
  name: domain
  type: string
- description: Name of the organization.
  name: organization
  type: string
- description: ''
  name: emails_count
  type: object
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-discover-result-schema.json
slug: hunter-discover-result
source_filename: hunter-discover-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DiscoverResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Domain name of the discovered company.\"\n    },\n    \"organization\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the organization.\"\n    },\n    \"emails_count\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-discover-result-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: DiscoverResult
---
