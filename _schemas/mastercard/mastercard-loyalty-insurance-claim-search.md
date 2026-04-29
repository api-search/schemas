---
description: ''
layout: schema
name: ClaimSearch
properties_list:
- description: Insurance claim identifier, cardholder should be able to retrieve once the claim is submitted on the target website.
  name: claimId
  type: string
- description: Postal code associated with insurance claim.
  name: postalCode
  type: string
- description: User's preferred language in localized ISO 639-1 format such as pt-BR
  name: preferredLanguage
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-loyalty-insurance-claim-search-schema.json
slug: mastercard-loyalty-insurance-claim-search
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClaimSearch\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"claimId\": {\n      \"type\": \"string\",\n      \"description\": \"Insurance claim identifier, cardholder should be able to retrieve once the claim is submitted on the target website.\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal code associated with insurance claim.\"\n    },\n    \"preferredLanguage\": {\n      \"type\": \"string\",\n      \"description\": \"User's preferred language in localized ISO 639-1 format such as pt-BR\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-loyalty-insurance-claim-search-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: ClaimSearch
---
