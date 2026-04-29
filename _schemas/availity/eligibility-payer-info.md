---
description: PayerInfo schema from Availity API
layout: schema
name: PayerInfo
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: address
  type: object
provider_name: availity
provider_slug: availity
schema_file: json-schema/eligibility-payer-info-schema.json
slug: eligibility-payer-info
source_filename: eligibility-payer-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-payer-info-schema.json\",\n  \"title\": \"PayerInfo\",\n  \"description\": \"PayerInfo schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"address1\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"state\": {\n          \"type\": \"string\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-payer-info-schema.json
tags: []
title: PayerInfo
---
