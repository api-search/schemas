---
description: ''
layout: schema
name: ForgotPassword-ChangePasswordRequest
properties_list:
- description: ''
  name: username
  type: string
- description: ''
  name: newpassword
  type: string
- description: ''
  name: otp
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-forgot-password-change-password-request-schema.json
slug: salesforce-forgot-password-change-password-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"newpassword\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"otp\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"username\",\n    \"newpassword\",\n    \"otp\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ForgotPassword-ChangePasswordRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-forgot-password-change-password-request-schema.json
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
title: ForgotPassword-ChangePasswordRequest
---
