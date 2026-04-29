---
description: ''
layout: schema
name: Source
properties_list:
- description: Domain where the email was found.
  name: domain
  type: string
- description: URL of the source page.
  name: uri
  type: string
- description: Date the email was extracted from the source.
  name: extracted_on
  type: string
- description: Date the email was last seen at the source.
  name: last_seen_on
  type: string
- description: Whether the email is still present on the source page.
  name: still_on_page
  type: boolean
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-source-schema.json
slug: hunter-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Source\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Domain where the email was found.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the source page.\"\n    },\n    \"extracted_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date the email was extracted from the source.\"\n    },\n    \"last_seen_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date the email was last seen at the source.\"\n    },\n    \"still_on_page\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email is still present on the source page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-source-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: Source
---
