---
description: TaxProfile schema from Avalara API
layout: schema
name: TaxProfile
properties_list:
- description: ''
  name: profileId
  type: integer
- description: ''
  name: profileName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: bundles
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-tax-profile-schema.json
slug: communications-tax-profile
source_filename: communications-tax-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-tax-profile-schema.json\",\n  \"title\": \"TaxProfile\",\n  \"description\": \"TaxProfile schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profileId\": {\n      \"type\": \"integer\"\n    },\n    \"profileName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"bundles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"bundleId\": {\n            \"type\": \"integer\"\n          },\n          \"bundleName\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-tax-profile-schema.json
tags:
- Taxes
title: TaxProfile
---
