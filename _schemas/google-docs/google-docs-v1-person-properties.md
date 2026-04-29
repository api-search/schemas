---
description: Properties specific to a linked person.
layout: schema
name: PersonProperties
properties_list:
- description: Output only. The name of the person.
  name: name
  type: string
- description: Output only. The email address linked to this person.
  name: email
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-person-properties-schema.json
slug: google-docs-v1-person-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PersonProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties specific to a linked person.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The name of the person.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The email address linked to this person.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-person-properties-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: PersonProperties
---
