---
description: ''
layout: schema
name: CompanySearchRequest
properties_list:
- description: ''
  name: metroRegion
  type: string
- description: ''
  name: industryCodes
  type: string
- description: ''
  name: techAttributeTagList
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-company-search-request-schema.json
slug: zoominfo-company-search-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"metroRegion\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"industryCodes\": {\n      \"type\": \"string\",\n      \"example\": \"Software\"\n    },\n    \"techAttributeTagList\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"metroRegion\",\n    \"industryCodes\",\n    \"techAttributeTagList\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompanySearchRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-company-search-request-schema.json
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
title: CompanySearchRequest
---
