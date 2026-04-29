---
description: ''
layout: schema
name: QuoteTermReaderAPIRequest
properties_list:
- description: ''
  name: context
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-quote-term-reader-api-request-schema.json
slug: salesforce-quote-term-reader-api-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"context\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"templateId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"language\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"templateId\",\n        \"language\"\n      ]\n    }\n  },\n  \"required\": [\n    \"context\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QuoteTermReaderAPIRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-quote-term-reader-api-request-schema.json
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
title: QuoteTermReaderAPIRequest
---
