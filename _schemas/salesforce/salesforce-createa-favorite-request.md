---
description: ''
layout: schema
name: CreateaFavoriteRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: sortOrder
  type: integer
- description: ''
  name: target
  type: string
- description: ''
  name: targetType
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-createa-favorite-request-schema.json
slug: salesforce-createa-favorite-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"sortOrder\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"target\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"targetType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"sortOrder\",\n    \"target\",\n    \"targetType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateaFavoriteRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-createa-favorite-request-schema.json
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
title: CreateaFavoriteRequest
---
