---
description: RelayedAuthorisationData schema from Adyen API
layout: schema
name: RelayedAuthorisationData
properties_list:
- description: Contains key-value pairs of your references and descriptions, for example, `customId`:`your-own-custom-field-12345`.
  name: metadata
  type: object
- description: Your reference for the relayed authorisation data.
  name: reference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-relayed-authorisation-data-schema.json
slug: transfers-relayed-authorisation-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-relayed-authorisation-data-schema.json\",\n  \"title\": \"RelayedAuthorisationData\",\n  \"description\": \"RelayedAuthorisationData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadata\": {\n      \"x-addedInVersion\": \"3\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Contains key-value pairs of your references and descriptions, for example, `customId`:`your-own-custom-field-12345`.\",\n      \"type\": \"object\"\n    },\n    \"reference\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Your reference for the relayed authorisation data.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-relayed-authorisation-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RelayedAuthorisationData
---
