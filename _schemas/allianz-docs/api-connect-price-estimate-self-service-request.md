---
description: Request body for creating a self-service price estimate session
layout: schema
name: PriceEstimateSelfServiceRequest
properties_list:
- description: Type of insurance product for the estimate
  name: product_type
  type: string
- description: ''
  name: vehicle
  type: object
- description: Age of the primary driver for car insurance
  name: driver_age
  type: integer
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-price-estimate-self-service-request-schema.json
slug: api-connect-price-estimate-self-service-request
source_filename: api-connect-price-estimate-self-service-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-price-estimate-self-service-request-schema.json\",\n  \"title\": \"PriceEstimateSelfServiceRequest\",\n  \"description\": \"Request body for creating a self-service price estimate session\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of insurance product for the estimate\",\n      \"enum\": [\n        \"home\",\n        \"landlord\",\n        \"car\"\n      ],\n      \"example\": \"car\"\n    },\n    \"vehicle\": {\n      \"$ref\": \"#/components/schemas/Vehicle\"\n    },\n    \"driver_age\": {\n      \"type\": \"integer\",\n      \"description\": \"Age of the primary driver for car insurance\",\n      \"example\": 35\n    }\n  },\n  \"required\": [\n    \"product_type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-price-estimate-self-service-request-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: PriceEstimateSelfServiceRequest
---
