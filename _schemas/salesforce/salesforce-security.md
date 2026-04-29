---
description: ''
layout: schema
name: Security
properties_list:
- description: ''
  name: bearerAuth
  type: array
- description: ''
  name: oAuth2
  type: array
- description: ''
  name: openIDConnectDiscovery
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-security-schema.json
slug: salesforce-security
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"bearerAuth\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"oAuth2\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"openIDConnectDiscovery\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Security\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-security-schema.json
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
title: Security
---
