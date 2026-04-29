---
description: ''
layout: schema
name: ForgotPassword-InitializeRequest
properties_list:
- description: ''
  name: username
  type: string
- description: ''
  name: recaptcha
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-forgot-password-initialize-request-schema.json
slug: salesforce-forgot-password-initialize-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"recaptcha\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"username\",\n    \"recaptcha\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ForgotPassword-InitializeRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-forgot-password-initialize-request-schema.json
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
title: ForgotPassword-InitializeRequest
---
