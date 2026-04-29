---
description: Represents a section within an item used to organize fields into logical groups.
layout: schema
name: Section
properties_list:
- description: The unique identifier for the section.
  name: id
  type: string
- description: The human-readable label for the section.
  name: label
  type: string
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-connect-section-schema.json
slug: 1password-connect-section
source_filename: 1password-connect-section-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-section-schema.json\",\n  \"title\": \"Section\",\n  \"description\": \"Represents a section within an item used to organize fields into logical groups.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the section.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable label for the section.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-section-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: Section
---
