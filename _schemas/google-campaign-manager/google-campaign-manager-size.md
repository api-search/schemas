---
description: Represents the dimensions of ads, placements, and creatives.
layout: schema
name: Size
properties_list:
- description: ID of this size.
  name: id
  type: string
- description: Width of this size in pixels.
  name: width
  type: integer
- description: Height of this size in pixels.
  name: height
  type: integer
- description: Whether this size is an IAB standard size.
  name: iab
  type: boolean
- description: ''
  name: kind
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-size-schema.json
slug: google-campaign-manager-size
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Size\",\n  \"type\": \"object\",\n  \"description\": \"Represents the dimensions of ads, placements, and creatives.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of this size.\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Width of this size in pixels.\"\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"Height of this size in pixels.\"\n    },\n    \"iab\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this size is an IAB standard size.\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-size-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: Size
---
