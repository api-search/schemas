---
description: A reference to a section within an item.
layout: schema
name: SectionRef
properties_list:
- description: The unique identifier of the referenced section.
  name: id
  type: string
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-connect-section-ref-schema.json
slug: 1password-connect-section-ref
source_filename: 1password-connect-section-ref-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-section-ref-schema.json\",\n  \"title\": \"SectionRef\",\n  \"description\": \"A reference to a section within an item.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the referenced section.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-section-ref-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: SectionRef
---
