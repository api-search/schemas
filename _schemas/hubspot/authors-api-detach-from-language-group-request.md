---
description: Request to detach an author from a multi-language group
layout: schema
name: DetachFromLanguageGroupRequest
properties_list:
- description: ID of the author to detach
  name: id
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/authors-api-detach-from-language-group-request-schema.json
slug: authors-api-detach-from-language-group-request
source_filename: authors-api-detach-from-language-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-detach-from-language-group-request-schema.json\",\n  \"title\": \"DetachFromLanguageGroupRequest\",\n  \"description\": \"Request to detach an author from a multi-language group\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the author to detach\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-detach-from-language-group-request-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: DetachFromLanguageGroupRequest
---
