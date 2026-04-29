---
description: ''
layout: schema
name: DeleteOrderRequest
properties_list:
- description: Order sequence number to delete
  name: EMSX_SEQUENCE
  type: integer
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-delete-order-request-schema.json
slug: bloomberg-emsx-delete-order-request
source_filename: bloomberg-emsx-delete-order-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteOrderRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_SEQUENCE\": {\n      \"type\": \"integer\",\n      \"description\": \"Order sequence number to delete\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-delete-order-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: DeleteOrderRequest
---
