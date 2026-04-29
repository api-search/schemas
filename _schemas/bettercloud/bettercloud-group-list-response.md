---
description: Paginated list of groups.
layout: schema
name: GroupListResponse
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: meta
  type: object
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-group-list-response-schema.json
slug: bettercloud-group-list-response
source_filename: bettercloud-group-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-group-list-response-schema.json\",\n  \"title\": \"GroupListResponse\",\n  \"description\": \"Paginated list of groups.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Group\"\n      }\n    },\n    \"meta\": {\n      \"$ref\": \"#/components/schemas/MetaResponse\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-group-list-response-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: GroupListResponse
---
