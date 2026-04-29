---
description: ''
layout: schema
name: AccountCreate
properties_list:
- description: ''
  name: Record
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-account-create-schema.json
slug: salesforce-account-create
source_filename: salesforce-account-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Record\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"Name\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"value\"\n          ]\n        }\n      },\n      \"required\": [\n        \"Id\",\n        \"Name\"\n      ]\n    }\n  },\n  \"required\": [\n    \"Record\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountCreate\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-account-create-schema.json
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
title: AccountCreate
---
