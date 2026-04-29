---
description: ''
layout: schema
name: MobileSDK
properties_list:
- description: ''
  name: UseiOSNativeBrowserForAuthentication
  type: boolean
- description: ''
  name: UseAndroidNativeBrowserForAuthentication
  type: boolean
- description: ''
  name: shareBrowserSessionIOS
  type: boolean
- description: ''
  name: shareBrowserSessionAndroid
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-mobile-sdk-schema.json
slug: salesforce-mobile-sdk
source_filename: salesforce-mobile-sdk-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UseiOSNativeBrowserForAuthentication\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"UseAndroidNativeBrowserForAuthentication\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"shareBrowserSessionIOS\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"shareBrowserSessionAndroid\": {\n      \"type\": \"boolean\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"UseiOSNativeBrowserForAuthentication\",\n    \"UseAndroidNativeBrowserForAuthentication\",\n    \"shareBrowserSessionIOS\",\n    \"shareBrowserSessionAndroid\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MobileSDK\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-mobile-sdk-schema.json
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
title: MobileSDK
---
