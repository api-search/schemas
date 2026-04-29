---
description: AddressRequirement schema from Adyen API
layout: schema
name: AddressRequirement
properties_list:
- description: Specifies the required address related fields for a particular route.
  name: description
  type: string
- description: List of address fields.
  name: requiredAddressFields
  type: array
- description: '**addressRequirement**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-address-requirement-schema.json
slug: configuration-address-requirement
source_filename: configuration-address-requirement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-address-requirement-schema.json\",\n  \"title\": \"AddressRequirement\",\n  \"description\": \"AddressRequirement schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"Specifies the required address related fields for a particular route.\",\n      \"type\": \"string\"\n    },\n    \"requiredAddressFields\": {\n      \"description\": \"List of address fields.\",\n      \"items\": {\n        \"enum\": [\n          \"city\",\n          \"country\",\n          \"line1\",\n          \"postalCode\",\n          \"stateOrProvince\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"type\": {\n      \"default\": \"addressRequirement\",\n      \"description\": \"**addressRequirement**\",\n      \"enum\"\
  : [\n        \"addressRequirement\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-address-requirement-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AddressRequirement
---
