---
description: ''
layout: schema
name: UpdateaFavoriteRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: sortOrder
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-updatea-favorite-request-schema.json
slug: salesforce-updatea-favorite-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"sortOrder\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"sortOrder\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateaFavoriteRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-updatea-favorite-request-schema.json
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
title: UpdateaFavoriteRequest
---
