---
description: ''
layout: schema
name: SuccessfulListNamedCredentials
properties_list:
- description: ''
  name: namedCredentials
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-list-named-credentials-schema.json
slug: salesforce-successful-list-named-credentials
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"namedCredentials\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"calloutUrl\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          },\n          \"developerName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"masterLabel\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          }\n        },\n        \"\
  required\": [\n          \"calloutUrl\",\n          \"developerName\",\n          \"id\",\n          \"masterLabel\",\n          \"type\",\n          \"url\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"namedCredentials\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulListNamedCredentials\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-list-named-credentials-schema.json
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
title: SuccessfulListNamedCredentials
---
