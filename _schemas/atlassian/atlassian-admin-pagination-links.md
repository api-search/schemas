---
description: Links for cursor-based pagination.
layout: schema
name: PaginationLinks
properties_list:
- description: Link to the current page.
  name: self
  type: string
- description: Link to the next page of results.
  name: next
  type: string
- description: Link to the previous page of results.
  name: prev
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-pagination-links-schema.json
slug: atlassian-admin-pagination-links
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaginationLinks\",\n  \"type\": \"object\",\n  \"description\": \"Links for cursor-based pagination.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\",\n      \"description\": \"Link to the current page.\"\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"description\": \"Link to the next page of results.\"\n    },\n    \"prev\": {\n      \"type\": \"string\",\n      \"description\": \"Link to the previous page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-pagination-links-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: PaginationLinks
---
