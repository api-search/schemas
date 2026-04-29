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
schema_file: json-schema/hubspot-authors-detach-from-language-group-request-schema.json
slug: hubspot-authors-detach-from-language-group-request
source_filename: hubspot-authors-detach-from-language-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request to detach an author from a multi-language group\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the author to detach\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DetachFromLanguageGroupRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-authors-detach-from-language-group-request-schema.json
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
