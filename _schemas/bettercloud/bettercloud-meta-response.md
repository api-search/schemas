---
description: Pagination metadata for list responses.
layout: schema
name: MetaResponse
properties_list:
- description: Current page number.
  name: page
  type: integer
- description: Number of items per page.
  name: per_page
  type: integer
- description: Total number of items.
  name: total
  type: integer
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-meta-response-schema.json
slug: bettercloud-meta-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-meta-response-schema.json\",\n  \"title\": \"MetaResponse\",\n  \"description\": \"Pagination metadata for list responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number.\",\n      \"example\": 1\n    },\n    \"per_page\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of items per page.\",\n      \"example\": 25\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of items.\",\n      \"example\": 150\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-meta-response-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: MetaResponse
---
