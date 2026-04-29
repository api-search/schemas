---
description: ''
layout: schema
name: ServiceProviderConfig
properties_list:
- description: ''
  name: schemas
  type: array
- description: An HTTP-addressable URL pointing to the service provider's human-consumable help documentation.
  name: documentationUri
  type: string
- description: A complex type that specifies PATCH configuration options.
  name: patch
  type: object
- description: A complex type that specifies bulk configuration options.
  name: bulk
  type: object
- description: A complex type that specifies FILTER options.
  name: filter
  type: object
- description: A complex type that specifies configuration options related to changing a password.
  name: changePassword
  type: object
- description: A complex type that specifies sort result options.
  name: sort
  type: object
- description: A complex type that specifies ETag configuration options.
  name: etag
  type: object
- description: A complex type that specifies supported authentication scheme properties.
  name: authenticationSchemes
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-procure-to-pay-scim-service-provider-config-schema.json
slug: factset-procure-to-pay-scim-service-provider-config
source_filename: factset-procure-to-pay-scim-service-provider-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceProviderConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\"\n    },\n    \"documentationUri\": {\n      \"type\": \"string\",\n      \"description\": \"An HTTP-addressable URL pointing to the service provider's human-consumable help documentation.\"\n    },\n    \"patch\": {\n      \"type\": \"object\",\n      \"description\": \"A complex type that specifies PATCH configuration options.\"\n    },\n    \"bulk\": {\n      \"type\": \"object\",\n      \"description\": \"A complex type that specifies bulk configuration options.\"\n    },\n    \"filter\": {\n      \"type\": \"object\",\n      \"description\": \"A complex type that specifies FILTER options.\"\n    },\n    \"changePassword\": {\n      \"type\": \"object\",\n      \"description\": \"A complex type that specifies configuration options related to changing a password.\"\n    },\n\
  \    \"sort\": {\n      \"type\": \"object\",\n      \"description\": \"A complex type that specifies sort result options.\"\n    },\n    \"etag\": {\n      \"type\": \"object\",\n      \"description\": \"A complex type that specifies ETag configuration options.\"\n    },\n    \"authenticationSchemes\": {\n      \"type\": \"object\",\n      \"description\": \"A complex type that specifies supported authentication scheme properties.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-procure-to-pay-scim-service-provider-config-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ServiceProviderConfig
---
