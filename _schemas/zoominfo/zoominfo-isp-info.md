---
description: ''
layout: schema
name: IspInfo
properties_list:
- description: ''
  name: domain
  type: string
- description: ''
  name: ip_hi_string
  type: string
- description: ''
  name: ip_lo_string
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-isp-info-schema.json
slug: zoominfo-isp-info
source_filename: zoominfo-isp-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"example\": \"example.com\"\n    },\n    \"ip_hi_string\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"ip_lo_string\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    }\n  },\n  \"required\": [\n    \"domain\",\n    \"ip_hi_string\",\n    \"ip_lo_string\",\n    \"name\",\n    \"type\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IspInfo\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-isp-info-schema.json
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
title: IspInfo
---
