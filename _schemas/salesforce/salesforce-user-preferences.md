---
description: ''
layout: schema
name: UserPreferences
properties_list:
- description: ''
  name: columnWidths
  type: object
- description: ''
  name: columnWrap
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-user-preferences-schema.json
slug: salesforce-user-preferences
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"columnWidths\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Site\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Type\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"BillingCountry\": {\n          \"type\": \"integer\",\n          \"example\": 42\n        },\n        \"Owner.Alias\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Phone\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Name\": {\n          \"type\": \"integer\",\n          \"example\": \"Example Title\"\n        }\n      },\n      \"required\": [\n        \"Site\",\n        \"Type\",\n        \"BillingCountry\",\n        \"Owner.Alias\",\n        \"Phone\",\n        \"Name\"\n      ]\n    },\n    \"columnWrap\": {\n      \"type\": \"object\",\n      \"properties\": {\n     \
  \   \"Site\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"Type\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"BillingCountry\": {\n          \"type\": \"boolean\",\n          \"example\": 42\n        },\n        \"Owner.Alias\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"Phone\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"Name\": {\n          \"type\": \"boolean\",\n          \"example\": \"Example Title\"\n        }\n      },\n      \"required\": [\n        \"Site\",\n        \"Type\",\n        \"BillingCountry\",\n        \"Owner.Alias\",\n        \"Phone\",\n        \"Name\"\n      ]\n    }\n  },\n  \"required\": [\n    \"columnWidths\",\n    \"columnWrap\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserPreferences\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-user-preferences-schema.json
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
title: UserPreferences
---
