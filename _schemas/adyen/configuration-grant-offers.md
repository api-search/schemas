---
description: GrantOffers schema from Adyen API
layout: schema
name: GrantOffers
properties_list:
- description: A list of available grant offers.
  name: grantOffers
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-grant-offers-schema.json
slug: configuration-grant-offers
source_filename: configuration-grant-offers-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-grant-offers-schema.json\",\n  \"title\": \"GrantOffers\",\n  \"description\": \"GrantOffers schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"grantOffers\": {\n      \"description\": \"A list of available grant offers.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/GrantOffer\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"grantOffers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-grant-offers-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GrantOffers
---
