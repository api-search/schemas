---
description: ''
layout: schema
name: AssociatedContact
properties_list:
- description: ''
  name: contactId
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-associated-contact-schema.json
slug: salesforce-associated-contact
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"contactId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"example\": \"user@example.com\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"contactId\",\n    \"email\",\n    \"firstName\",\n    \"lastName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssociatedContact\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-associated-contact-schema.json
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
title: AssociatedContact
---
