---
description: ''
layout: schema
name: SuccessfulSalesforceKeys
properties_list:
- description: ''
  name: keys
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-salesforce-keys-schema.json
slug: salesforce-successful-salesforce-keys
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"keys\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"kty\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"n\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"e\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"alg\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"use\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"kid\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"kty\",\n          \"n\",\n        \
  \  \"e\",\n          \"alg\",\n          \"use\",\n          \"kid\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"keys\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulSalesforceKeys\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-salesforce-keys-schema.json
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
title: SuccessfulSalesforceKeys
---
