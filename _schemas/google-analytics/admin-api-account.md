---
description: A resource message representing a Google Analytics account.
layout: schema
name: Account
properties_list:
- description: Output only. Time when this account was originally created.
  name: createTime
  type: string
- description: Output only. Indicates whether this Account is soft-deleted or not. Deleted accounts are excluded from List results unless specifically requested.
  name: deleted
  type: boolean
- description: Required. Human-readable display name for this account.
  name: displayName
  type: string
- description: 'Output only. Resource name of this account. Format: accounts/{account} Example: "accounts/100"'
  name: name
  type: string
- description: Country of business. Must be a Unicode CLDR region code.
  name: regionCode
  type: string
- description: Output only. Time when account payload fields were last updated.
  name: updateTime
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/admin-api-account-schema.json
slug: admin-api-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-account-schema.json\",\n  \"title\": \"Account\",\n  \"description\": \"A resource message representing a Google Analytics account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createTime\": {\n      \"description\": \"Output only. Time when this account was originally created.\",\n      \"format\": \"google-datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"deleted\": {\n      \"description\": \"Output only. Indicates whether this Account is soft-deleted or not. Deleted accounts are excluded from List results unless specifically requested.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"displayName\": {\n      \"description\": \"Required. Human-readable\
  \ display name for this account.\",\n      \"type\": \"string\",\n      \"example\": \"Example Name\"\n    },\n    \"name\": {\n      \"description\": \"Output only. Resource name of this account. Format: accounts/{account} Example: \\\"accounts/100\\\"\",\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"example\": \"Example Name\"\n    },\n    \"regionCode\": {\n      \"description\": \"Country of business. Must be a Unicode CLDR region code.\",\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"updateTime\": {\n      \"description\": \"Output only. Time when account payload fields were last updated.\",\n      \"format\": \"google-datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-account-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: Account
---
