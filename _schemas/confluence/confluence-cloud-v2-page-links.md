---
description: ''
layout: schema
name: PageLinks
properties_list:
- description: Web UI link for the page.
  name: webui
  type: string
- description: Edit UI link for the page.
  name: editui
  type: string
- description: Shortened link for the page.
  name: tinyui
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-page-links-schema.json
slug: confluence-cloud-v2-page-links
source_filename: confluence-cloud-v2-page-links-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PageLinks\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"webui\": {\n      \"type\": \"string\",\n      \"description\": \"Web UI link for the page.\"\n    },\n    \"editui\": {\n      \"type\": \"string\",\n      \"description\": \"Edit UI link for the page.\"\n    },\n    \"tinyui\": {\n      \"type\": \"string\",\n      \"description\": \"Shortened link for the page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-page-links-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: PageLinks
---
