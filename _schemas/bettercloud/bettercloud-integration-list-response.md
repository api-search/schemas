---
description: List of configured SaaS integrations.
layout: schema
name: IntegrationListResponse
properties_list:
- description: ''
  name: data
  type: array
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-integration-list-response-schema.json
slug: bettercloud-integration-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-integration-list-response-schema.json\",\n  \"title\": \"IntegrationListResponse\",\n  \"description\": \"List of configured SaaS integrations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Integration\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-integration-list-response-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: IntegrationListResponse
---
