---
description: ''
layout: schema
name: GetApps
properties_list:
- description: ''
  name: apps
  type: array
- description: ''
  name: eTag
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-get-apps-schema.json
slug: salesforce-get-apps
source_filename: salesforce-get-apps-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"apps\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"appId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"example\": \"A sample description.\"\n          },\n          \"developerName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"eTag\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"formFactors\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"headerColor\": {\n            \"type\": \"string\"\
  ,\n            \"example\": \"example_value\"\n          },\n          \"iconUrl\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"https://www.example.com\"\n          },\n          \"isNavAutoTempTabsDisabled\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"isNavPersonalizationDisabled\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"isNavTabPersistenceDisabled\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"logoUrl\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          },\n          \"mobileStartUrl\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"https://www.example.com\"\n          },\n          \"navItems\":\
  \ {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\"\n            }\n          },\n          \"selected\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"startUrl\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"userNavItems\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"required\": [\n          \"appId\",\n          \"description\",\n          \"developerName\",\n          \"eTag\",\n          \"formFactors\",\n          \"headerColor\",\n          \"iconUrl\",\n          \"\
  isNavAutoTempTabsDisabled\",\n          \"isNavPersonalizationDisabled\",\n          \"isNavTabPersistenceDisabled\",\n          \"label\",\n          \"logoUrl\",\n          \"mobileStartUrl\",\n          \"navItems\",\n          \"selected\",\n          \"startUrl\",\n          \"type\",\n          \"userNavItems\"\n        ]\n      }\n    },\n    \"eTag\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"apps\",\n    \"eTag\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetApps\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-get-apps-schema.json
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
title: GetApps
---
