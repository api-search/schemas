---
description: ''
layout: schema
name: GetOrdersRequest
properties_list:
- description: Scope of orders to retrieve
  name: scope
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-get-orders-request-schema.json
slug: bloomberg-emsx-get-orders-request
source_filename: bloomberg-emsx-get-orders-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetOrdersRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"Scope of orders to retrieve\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-get-orders-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: GetOrdersRequest
---
