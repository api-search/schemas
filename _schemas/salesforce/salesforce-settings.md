---
description: ''
layout: schema
name: Settings
properties_list:
- description: ''
  name: maxMiddleValues
  type: integer
- description: ''
  name: maxPrescriptions
  type: integer
- description: ''
  name: prescriptionImpactPercentage
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-settings-schema.json
slug: salesforce-settings
source_filename: salesforce-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxMiddleValues\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"maxPrescriptions\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"prescriptionImpactPercentage\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"maxMiddleValues\",\n    \"maxPrescriptions\",\n    \"prescriptionImpactPercentage\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Settings\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-settings-schema.json
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
title: Settings
---
