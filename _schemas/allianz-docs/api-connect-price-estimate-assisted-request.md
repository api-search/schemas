---
description: Request body for creating a staff-assisted price estimate
layout: schema
name: PriceEstimateAssistedRequest
properties_list:
- description: Unique identifier for the customer
  name: customer_id
  type: string
- description: Type of insurance product to estimate
  name: product_type
  type: string
- description: ''
  name: property_address
  type: object
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-price-estimate-assisted-request-schema.json
slug: api-connect-price-estimate-assisted-request
source_filename: api-connect-price-estimate-assisted-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-price-estimate-assisted-request-schema.json\",\n  \"title\": \"PriceEstimateAssistedRequest\",\n  \"description\": \"Request body for creating a staff-assisted price estimate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customer_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the customer\",\n      \"example\": \"500123\"\n    },\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of insurance product to estimate\",\n      \"enum\": [\n        \"home\",\n        \"landlord\",\n        \"car\"\n      ],\n      \"example\": \"home\"\n    },\n    \"property_address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    }\n  },\n  \"required\": [\n    \"customer_id\",\n    \"product_type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-price-estimate-assisted-request-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: PriceEstimateAssistedRequest
---
