---
description: Quota configuration for an offering item
layout: schema
name: Quota
properties_list:
- description: Quota value (null for unlimited)
  name: value
  type: number
- description: Allowed overage beyond quota
  name: overage
  type: number
- description: Quota version for concurrency
  name: version
  type: integer
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/account-management-quota-schema.json
slug: account-management-quota
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-quota-schema.json\",\n  \"title\": \"Quota\",\n  \"description\": \"Quota configuration for an offering item\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Quota value (null for unlimited)\",\n      \"example\": 100\n    },\n    \"overage\": {\n      \"type\": \"number\",\n      \"description\": \"Allowed overage beyond quota\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Quota version for concurrency\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-quota-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: Quota
---
