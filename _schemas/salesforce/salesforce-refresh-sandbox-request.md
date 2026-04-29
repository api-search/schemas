---
description: ''
layout: schema
name: RefreshSandboxRequest
properties_list:
- description: ''
  name: LicenseType
  type: string
- description: ''
  name: AutoActivate
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-refresh-sandbox-request-schema.json
slug: salesforce-refresh-sandbox-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"LicenseType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"AutoActivate\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"LicenseType\",\n    \"AutoActivate\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RefreshSandboxRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-refresh-sandbox-request-schema.json
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
title: RefreshSandboxRequest
---
