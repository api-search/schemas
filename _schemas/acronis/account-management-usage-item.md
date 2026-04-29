---
description: Usage metric for a specific service or resource
layout: schema
name: UsageItem
properties_list:
- description: Name of the offering item
  name: offering_item
  type: string
- description: ''
  name: application_id
  type: string
- description: Current usage value
  name: value
  type: number
- description: ''
  name: edition
  type: string
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/account-management-usage-item-schema.json
slug: account-management-usage-item
source_filename: account-management-usage-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-usage-item-schema.json\",\n  \"title\": \"UsageItem\",\n  \"description\": \"Usage metric for a specific service or resource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"offering_item\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the offering item\",\n      \"example\": \"vms\"\n    },\n    \"application_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Current usage value\",\n      \"example\": 42\n    },\n    \"edition\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-usage-item-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: UsageItem
---
