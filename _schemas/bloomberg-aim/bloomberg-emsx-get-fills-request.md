---
description: ''
layout: schema
name: GetFillsRequest
properties_list:
- description: ''
  name: scope
  type: string
- description: Start of time range for fills
  name: fromDateTime
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-get-fills-request-schema.json
slug: bloomberg-emsx-get-fills-request
source_filename: bloomberg-emsx-get-fills-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetFillsRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scope\": {\n      \"type\": \"string\"\n    },\n    \"fromDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Start of time range for fills\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-get-fills-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: GetFillsRequest
---
