---
description: ''
layout: schema
name: SuccessfulFilesSharesLink
properties_list:
- description: ''
  name: expirationDate
  type: '[''string'', ''null'']'
- description: ''
  name: fileViewUrl
  type: string
- description: ''
  name: isPasswordRequired
  type: boolean
- description: ''
  name: password
  type: '[''string'', ''null'']'
- description: ''
  name: sharingType
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-files-shares-link-schema.json
slug: salesforce-successful-files-shares-link
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"expirationDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"fileViewUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"isPasswordRequired\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"password\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"sharingType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"expirationDate\",\n    \"fileViewUrl\",\n    \"isPasswordRequired\",\n    \"password\",\n    \"sharingType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulFilesSharesLink\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-files-shares-link-schema.json
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
title: SuccessfulFilesSharesLink
---
