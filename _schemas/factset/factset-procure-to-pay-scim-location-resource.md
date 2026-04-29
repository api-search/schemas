---
description: ''
layout: schema
name: LocationResource
properties_list:
- description: ''
  name: schemas
  type: array
- description: ''
  name: id
  type: string
- description: ''
  name: externalId
  type: string
- description: Name of the location.
  name: name
  type: string
- description: Description of the location.
  name: description
  type: string
- description: First line of location's address.
  name: address1
  type: string
- description: Second line of location's address.
  name: address2
  type: string
- description: Third line of location's address.
  name: address3
  type: string
- description: City of location.
  name: locality
  type: string
- description: State or province of location.
  name: region
  type: string
- description: Postal code of location.
  name: postalCode
  type: string
- description: Country of location.
  name: country
  type: string
- description: Phone number of location.
  name: phoneNumber
  type: string
- description: ''
  name: mainLocation
  type: string
- description: ''
  name: meta
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-procure-to-pay-scim-location-resource-schema.json
slug: factset-procure-to-pay-scim-location-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LocationResource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"externalId\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the location.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the location.\"\n    },\n    \"address1\": {\n      \"type\": \"string\",\n      \"description\": \"First line of location's address.\"\n    },\n    \"address2\": {\n      \"type\": \"string\",\n      \"description\": \"Second line of location's address.\"\n    },\n    \"address3\": {\n      \"type\": \"string\",\n      \"description\": \"Third line of location's address.\"\n    },\n    \"locality\": {\n      \"type\": \"string\",\n      \"description\": \"City of location.\"\
  \n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"State or province of location.\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal code of location.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country of location.\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number of location.\"\n    },\n    \"mainLocation\": {\n      \"type\": \"string\"\n    },\n    \"meta\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-procure-to-pay-scim-location-resource-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: LocationResource
---
