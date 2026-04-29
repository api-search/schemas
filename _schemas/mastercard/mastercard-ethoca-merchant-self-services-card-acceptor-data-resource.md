---
description: ''
layout: schema
name: CardAcceptorDataResource
properties_list:
- description: The card acceptor match type
  name: matchType
  type: string
- description: The status of Card Acceptor Name - PENDING, PASS, FAILED
  name: status
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-card-acceptor-data-resource-schema.json
slug: mastercard-ethoca-merchant-self-services-card-acceptor-data-resource
source_filename: mastercard-ethoca-merchant-self-services-card-acceptor-data-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CardAcceptorDataResource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"matchType\": {\n      \"type\": \"string\",\n      \"description\": \"The card acceptor match type\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of Card Acceptor Name - PENDING, PASS, FAILED\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-card-acceptor-data-resource-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: CardAcceptorDataResource
---
