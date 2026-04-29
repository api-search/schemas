---
description: GrantOffer schema from Adyen API
layout: schema
name: GrantOffer
properties_list:
- description: The identifier of the account holder to which the grant is offered.
  name: accountHolderId
  type: string
- description: The principal amount of the grant.
  name: amount
  type: object
- description: 'The contract type of the grant offer. Possible value: **cashAdvance**, **loan**.'
  name: contractType
  type: string
- description: The end date of the grant offer validity period.
  name: expiresAt
  type: string
- description: Details of the fee configuration.
  name: fee
  type: object
- description: The unique identifier of the grant offer.
  name: id
  type: string
- description: Details of the repayment configuration.
  name: repayment
  type: object
- description: The starting date of the grant offer validity period.
  name: startsAt
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-grant-offer-schema.json
slug: configuration-grant-offer
source_filename: configuration-grant-offer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-grant-offer-schema.json\",\n  \"title\": \"GrantOffer\",\n  \"description\": \"GrantOffer schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderId\": {\n      \"description\": \"The identifier of the account holder to which the grant is offered.\",\n      \"type\": \"string\"\n    },\n    \"amount\": {\n      \"description\": \"The principal amount of the grant.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"contractType\": {\n      \"description\": \"The contract type of the grant offer. Possible value: **cashAdvance**, **loan**.\",\n      \"enum\": [\n        \"cashAdvance\",\n        \"loan\"\n      ],\n      \"type\": \"string\"\n    },\n    \"expiresAt\": {\n      \"description\": \"The end date of the grant offer validity period.\",\n \
  \     \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"fee\": {\n      \"description\": \"Details of the fee configuration.\",\n      \"$ref\": \"#/components/schemas/Fee\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the grant offer.\",\n      \"type\": \"string\"\n    },\n    \"repayment\": {\n      \"description\": \"Details of the repayment configuration.\",\n      \"$ref\": \"#/components/schemas/Repayment\"\n    },\n    \"startsAt\": {\n      \"description\": \"The starting date of the grant offer validity period.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountHolderId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-grant-offer-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GrantOffer
---
