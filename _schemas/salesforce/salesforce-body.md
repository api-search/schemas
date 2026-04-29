---
description: ''
layout: schema
name: Body
properties_list:
- description: ''
  name: Name
  type: string
- description: ''
  name: LastName
  type: string
- description: ''
  name: AccountId
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-body-schema.json
slug: salesforce-body
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"LastName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"AccountId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Body\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-body-schema.json
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
title: Body
---
