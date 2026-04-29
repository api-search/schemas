---
description: ''
layout: schema
name: ColumnWrap
properties_list:
- description: ''
  name: Site
  type: boolean
- description: ''
  name: Type
  type: boolean
- description: ''
  name: BillingCountry
  type: boolean
- description: ''
  name: Owner.Alias
  type: boolean
- description: ''
  name: Phone
  type: boolean
- description: ''
  name: Name
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-column-wrap-schema.json
slug: salesforce-column-wrap
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Site\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"Type\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"BillingCountry\": {\n      \"type\": \"boolean\",\n      \"example\": 42\n    },\n    \"Owner.Alias\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"Phone\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"Name\": {\n      \"type\": \"boolean\",\n      \"example\": \"Example Title\"\n    }\n  },\n  \"required\": [\n    \"Site\",\n    \"Type\",\n    \"BillingCountry\",\n    \"Owner.Alias\",\n    \"Phone\",\n    \"Name\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ColumnWrap\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-column-wrap-schema.json
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
title: ColumnWrap
---
