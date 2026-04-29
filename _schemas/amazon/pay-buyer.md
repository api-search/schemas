---
description: Buyer schema from Amazon Pay API
layout: schema
name: Buyer
properties_list:
- description: ''
  name: buyerId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: email
  type: string
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/pay-buyer-schema.json
slug: pay-buyer
source_filename: pay-buyer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"buyerId\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Buyer\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-buyer-schema.json\",\n  \"description\": \"Buyer schema from Amazon Pay API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-buyer-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: Buyer
---
