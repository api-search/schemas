---
description: ''
layout: schema
name: PasswordlessLogin-InitializeRequest
properties_list:
- description: ''
  name: username
  type: string
- description: ''
  name: recaptcha
  type: string
- description: ''
  name: verificationmethod
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-passwordless-login-initialize-request-schema.json
slug: salesforce-passwordless-login-initialize-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"recaptcha\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"verificationmethod\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"username\",\n    \"recaptcha\",\n    \"verificationmethod\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PasswordlessLogin-InitializeRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-passwordless-login-initialize-request-schema.json
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
title: PasswordlessLogin-InitializeRequest
---
