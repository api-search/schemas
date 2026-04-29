---
description: ''
layout: schema
name: Verified
properties_list:
- description: ''
  name: isVerifiableByMe
  type: boolean
- description: ''
  name: isVerified
  type: boolean
- description: ''
  name: isVerifiedByAnonymized
  type: '[''string'', ''null'']'
- description: ''
  name: lastVerifiedByUser
  type: '[''string'', ''null'']'
- description: ''
  name: lastVerifiedDate
  type: '[''string'', ''null'']'
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-verified-schema.json
slug: salesforce-verified
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"isVerifiableByMe\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"isVerified\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"isVerifiedByAnonymized\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"lastVerifiedByUser\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"lastVerifiedDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"isVerifiableByMe\",\n    \"isVerified\",\n    \"isVerifiedByAnonymized\",\n    \"lastVerifiedByUser\",\n    \"lastVerifiedDate\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Verified\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-verified-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: Verified
---
