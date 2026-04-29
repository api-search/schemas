---
description: Schema for a sub-merchant logo status
layout: schema
name: LogoResource
properties_list:
- description: Status of the logo
  name: status
  type: string
- description: List of validation messages for a logo.
  name: messages
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-logo-resource-schema.json
slug: mastercard-ethoca-merchant-self-services-logo-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogoResource\",\n  \"type\": \"object\",\n  \"description\": \"Schema for a sub-merchant logo status\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the logo\"\n    },\n    \"messages\": {\n      \"type\": \"array\",\n      \"description\": \"List of validation messages for a logo.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-logo-resource-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: LogoResource
---
