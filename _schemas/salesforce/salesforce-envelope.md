---
description: ''
layout: schema
name: Envelope
properties_list:
- description: ''
  name: Header
  type: object
- description: ''
  name: Body
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-envelope-schema.json
slug: salesforce-envelope
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Header\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"Body\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"Header\",\n    \"Body\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Envelope\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-envelope-schema.json
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
title: Envelope
---
