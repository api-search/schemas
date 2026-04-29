---
description: An Acronis service or feature that can be enabled for a tenant
layout: schema
name: OfferingItem
properties_list:
- description: Offering item identifier name
  name: name
  type: string
- description: Application that provides this offering item
  name: application_id
  type: string
- description: Item status (1=active, 0=inactive)
  name: status
  type: integer
- description: ''
  name: quota
  type: object
- description: Edition name this item belongs to
  name: edition
  type: string
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/account-management-offering-item-schema.json
slug: account-management-offering-item
source_filename: account-management-offering-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-offering-item-schema.json\",\n  \"title\": \"OfferingItem\",\n  \"description\": \"An Acronis service or feature that can be enabled for a tenant\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Offering item identifier name\",\n      \"example\": \"vms\"\n    },\n    \"application_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Application that provides this offering item\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"Item status (1=active, 0=inactive)\",\n      \"example\": 1\n    },\n    \"quota\": {\n      \"$ref\": \"#/components/schemas/Quota\"\n    },\n    \"edition\": {\n      \"type\": \"string\",\n      \"description\": \"Edition\
  \ name this item belongs to\",\n      \"example\": \"standard\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-offering-item-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: OfferingItem
---
