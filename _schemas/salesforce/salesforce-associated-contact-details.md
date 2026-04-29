---
description: ''
layout: schema
name: AssociatedContactDetails
properties_list:
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: allowDuplicateRecords
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-associated-contact-details-schema.json
slug: salesforce-associated-contact-details
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"example\": \"user@example.com\"\n    },\n    \"allowDuplicateRecords\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"firstName\",\n    \"lastName\",\n    \"email\",\n    \"allowDuplicateRecords\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssociatedContactDetails\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-associated-contact-details-schema.json
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
title: AssociatedContactDetails
---
