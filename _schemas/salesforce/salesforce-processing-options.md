---
description: ''
layout: schema
name: ProcessingOptions
properties_list:
- description: ''
  name: donorOptions
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-processing-options-schema.json
slug: salesforce-processing-options
source_filename: salesforce-processing-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"donorOptions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"defaultUpdateLogic\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"defaultUpdateLogic\"\n      ]\n    }\n  },\n  \"required\": [\n    \"donorOptions\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProcessingOptions\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-processing-options-schema.json
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
title: ProcessingOptions
---
