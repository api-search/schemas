---
description: ''
layout: schema
name: Contacts
properties_list:
- description: ''
  name: records
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-contacts-schema.json
slug: salesforce-contacts
source_filename: salesforce-contacts-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"records\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"attributes\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"referenceId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              }\n            },\n            \"required\": [\n              \"type\",\n              \"referenceId\"\n            ]\n          },\n          \"lastname\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"Title\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"email\": {\n         \
  \   \"type\": \"string\",\n            \"example\": \"user@example.com\"\n          }\n        },\n        \"required\": [\n          \"attributes\",\n          \"lastname\",\n          \"email\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"records\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Contacts\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-contacts-schema.json
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
title: Contacts
---
