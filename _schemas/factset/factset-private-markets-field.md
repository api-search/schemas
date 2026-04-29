---
description: ''
layout: schema
name: field
properties_list:
- description: Data item to be used as `fields` input in `/factset-private-markets/v#/` endpoint.
  name: field
  type: string
- description: Plain text name of the field.
  name: name
  type: string
- description: 'Corresponding endpoint to input field item. For example, fields returning the category ''FINANCIALS'' should be used in the /financials endpoint. The same follows data items falling in the category for '
  name: category
  type: string
- description: The factor for the field (e.g. 1000 = thousands).
  name: factor
  type: integer
- description: The name of the data item as it appears in the Standard Data Feed (SDF). A null value represents items available only in API.
  name: sdfName
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-private-markets-field-schema.json
slug: factset-private-markets-field
source_filename: factset-private-markets-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"field\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"field\": {\n      \"type\": \"string\",\n      \"description\": \"Data item to be used as `fields` input in `/factset-private-markets/v#/` endpoint.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Plain text name of the field.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Corresponding endpoint to input field item. For example, fields returning the category 'FINANCIALS' should be used in the /financials endpoint. The same follows data items falling in the category for NON_PERIODIC, which would be used in the /non-periodic endpoint.\"\n    },\n    \"factor\": {\n      \"type\": \"integer\",\n      \"description\": \"The factor for the field (e.g. 1000 = thousands).\"\n    },\n    \"sdfName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of\
  \ the data item as it appears in the Standard Data Feed (SDF). A null value represents items available only in API.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-private-markets-field-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: field
---
