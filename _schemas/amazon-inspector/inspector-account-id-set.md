---
description: AccountIdSet schema
layout: schema
name: AccountIdSet
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-account-id-set-schema.json
slug: inspector-account-id-set
source_filename: inspector-account-id-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-account-id-set-schema.json\",\n  \"title\": \"AccountIdSet\",\n  \"description\": \"AccountIdSet schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"^\\\\d{12}$\",\n    \"minLength\": 12,\n    \"maxLength\": 12\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-account-id-set-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AccountIdSet
---
