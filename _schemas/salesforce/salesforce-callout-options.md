---
description: ''
layout: schema
name: CalloutOptions
properties_list:
- description: ''
  name: allowMergeFieldsInBody
  type: boolean
- description: ''
  name: allowMergeFieldsInHeader
  type: boolean
- description: ''
  name: generateAuthorizationHeader
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-callout-options-schema.json
slug: salesforce-callout-options
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowMergeFieldsInBody\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"allowMergeFieldsInHeader\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"generateAuthorizationHeader\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"allowMergeFieldsInBody\",\n    \"allowMergeFieldsInHeader\",\n    \"generateAuthorizationHeader\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CalloutOptions\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-callout-options-schema.json
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
title: CalloutOptions
---
