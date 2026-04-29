---
description: ''
layout: schema
name: GetCompanyRanking
properties_list:
- description: ''
  name: Id
  type: string
- description: ''
  name: Name
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-get-company-ranking-schema.json
slug: zoominfo-get-company-ranking
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    }\n  },\n  \"required\": [\n    \"Id\",\n    \"Name\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetCompanyRanking\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-get-company-ranking-schema.json
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
title: GetCompanyRanking
---
