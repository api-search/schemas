---
description: ''
layout: schema
name: BannerPhoto
properties_list:
- description: ''
  name: bannerPhotoUrl
  type: string
- description: ''
  name: bannerPhotoVersionId
  type: '[''string'', ''null'']'
- description: ''
  name: url
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-banner-photo-schema.json
slug: salesforce-banner-photo
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"bannerPhotoUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"bannerPhotoVersionId\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"500123\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"bannerPhotoUrl\",\n    \"bannerPhotoVersionId\",\n    \"url\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BannerPhoto\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-banner-photo-schema.json
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
title: BannerPhoto
---
