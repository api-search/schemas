---
description: ''
layout: schema
name: AuthenticateRequest
properties_list:
- description: ''
  name: username
  type: string
- description: ''
  name: password
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-authenticate-request-schema.json
slug: zoominfo-authenticate-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"example\": \"password\"\n    }\n  },\n  \"required\": [\n    \"username\",\n    \"password\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AuthenticateRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-authenticate-request-schema.json
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
title: AuthenticateRequest
---
