---
description: ''
layout: schema
name: SuccessfulAssetTokenFlow
properties_list:
- description: ''
  name: access_token
  type: string
- description: ''
  name: issued_token_type
  type: string
- description: ''
  name: token_type
  type: string
- description: ''
  name: expires_in
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-asset-token-flow-schema.json
slug: salesforce-successful-asset-token-flow
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    },\n    \"issued_token_type\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"access_token\",\n    \"issued_token_type\",\n    \"token_type\",\n    \"expires_in\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulAssetTokenFlow\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-asset-token-flow-schema.json
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
title: SuccessfulAssetTokenFlow
---
