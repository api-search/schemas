---
description: PaginationInfo schema from AhaSend API
layout: schema
name: PaginationInfo
properties_list:
- description: Whether there are more items available
  name: has_more
  type: boolean
- description: Cursor for the next page of results
  name: next_cursor
  type: string
- description: Cursor for the previous page of results
  name: previous_cursor
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-pagination-info-schema.json
slug: openapi-v2-pagination-info
source_filename: openapi-v2-pagination-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-pagination-info-schema.json\",\n  \"title\": \"PaginationInfo\",\n  \"description\": \"PaginationInfo schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"has_more\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether there are more items available\",\n      \"example\": true\n    },\n    \"next_cursor\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page of results\",\n      \"example\": \"example_value\"\n    },\n    \"previous_cursor\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the previous page of results\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"has_more\"\n  ],\n  \"example\": {\n    \"has_more\": true,\n    \"next_cursor\": \"eyJpZCI6MTIzNH0=\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-pagination-info-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: PaginationInfo
---
