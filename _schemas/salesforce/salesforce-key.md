---
description: ''
layout: schema
name: Key
properties_list:
- description: ''
  name: kty
  type: string
- description: ''
  name: n
  type: string
- description: ''
  name: e
  type: string
- description: ''
  name: alg
  type: string
- description: ''
  name: use
  type: string
- description: ''
  name: kid
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-key-schema.json
slug: salesforce-key
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"kty\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"n\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"e\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"alg\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"use\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"kid\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"kty\",\n    \"n\",\n    \"e\",\n    \"alg\",\n    \"use\",\n    \"kid\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Key\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-key-schema.json
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
title: Key
---
