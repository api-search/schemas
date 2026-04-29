---
description: ''
layout: schema
name: ReadProductAPIRequest
properties_list:
- description: ''
  name: context
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-read-product-api-request-schema.json
slug: salesforce-read-product-api-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"context\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"pricebookId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"currencyCode\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"pricebookId\",\n        \"currencyCode\"\n      ]\n    }\n  },\n  \"required\": [\n    \"context\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReadProductAPIRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-read-product-api-request-schema.json
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
title: ReadProductAPIRequest
---
