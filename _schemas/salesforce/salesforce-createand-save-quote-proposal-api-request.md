---
description: ''
layout: schema
name: CreateandSaveQuoteProposalAPIRequest
properties_list:
- description: ''
  name: saver
  type: string
- description: ''
  name: model
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-createand-save-quote-proposal-api-request-schema.json
slug: salesforce-createand-save-quote-proposal-api-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"saver\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"model\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"quoteId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"templateId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"outputFormat\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"language\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"paperSize\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"name\",\n        \"quoteId\",\n        \"templateId\",\n        \"outputFormat\"\
  ,\n        \"language\",\n        \"paperSize\"\n      ]\n    }\n  },\n  \"required\": [\n    \"saver\",\n    \"model\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateandSaveQuoteProposalAPIRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-createand-save-quote-proposal-api-request-schema.json
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
title: CreateandSaveQuoteProposalAPIRequest
---
