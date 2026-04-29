---
description: ExcludedAccounts schema
layout: schema
name: ExcludedAccounts
properties_list: []
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-excluded-accounts-schema.json
slug: config-excluded-accounts
source_filename: config-excluded-accounts-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-excluded-accounts-schema.json\",\n  \"title\": \"ExcludedAccounts\",\n  \"description\": \"ExcludedAccounts schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/AccountId\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 1000\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-excluded-accounts-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ExcludedAccounts
---
