---
description: An AppSumo software license purchased through the marketplace
layout: schema
name: License
properties_list:
- description: Unique license key for activation
  name: licenseKey
  type: string
- description: AppSumo product slug identifier
  name: productSlug
  type: string
- description: Current license status
  name: status
  type: string
- description: License tier (Tier 1, 2, 3, etc.)
  name: tier
  type: string
- description: When the license was activated
  name: activatedAt
  type: string
- description: AppSumo user who purchased the license
  name: userId
  type: string
- description: Purchaser email address
  name: email
  type: string
provider_name: AppSumo
provider_slug: appsumo
schema_file: json-schema/license-schema.json
slug: license
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appsumo/main/json-schema/license-schema.json\",\n  \"title\": \"License\",\n  \"description\": \"An AppSumo software license purchased through the marketplace\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"licenseKey\": {\n      \"type\": \"string\",\n      \"description\": \"Unique license key for activation\"\n    },\n    \"productSlug\": {\n      \"type\": \"string\",\n      \"description\": \"AppSumo product slug identifier\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"refunded\"\n      ],\n      \"description\": \"Current license status\"\n    },\n    \"tier\": {\n      \"type\": \"string\",\n      \"description\": \"License tier (Tier 1, 2, 3, etc.)\"\n    },\n    \"activatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n\
  \      \"description\": \"When the license was activated\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"AppSumo user who purchased the license\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Purchaser email address\"\n    }\n  },\n  \"required\": [\n    \"licenseKey\",\n    \"productSlug\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appsumo/refs/heads/main/json-schema/license-schema.json
tags:
- Marketplace
- SaaS
- Software Deals
title: License
---
