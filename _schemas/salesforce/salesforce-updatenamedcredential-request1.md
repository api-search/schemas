---
description: ''
layout: schema
name: UpdatenamedcredentialRequest1
properties_list:
- description: ''
  name: FullName
  type: string
- description: ''
  name: Metadata
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-updatenamedcredential-request1-schema.json
slug: salesforce-updatenamedcredential-request1
source_filename: salesforce-updatenamedcredential-request1-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"FullName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"endpoint\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"principalType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"protocol\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"label\",\n        \"endpoint\",\n        \"principalType\",\n        \"protocol\"\n      ]\n    }\n  },\n  \"required\": [\n    \"FullName\",\n    \"Metadata\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdatenamedcredentialRequest1\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-updatenamedcredential-request1-schema.json
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
title: UpdatenamedcredentialRequest1
---
