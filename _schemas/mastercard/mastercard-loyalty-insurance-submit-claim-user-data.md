---
description: ''
layout: schema
name: SubmitClaimUserData
properties_list:
- description: First name
  name: firstName
  type: string
- description: Last name
  name: lastName
  type: string
- description: Address line 1
  name: addressLine1
  type: string
- description: Address line 2
  name: addressLine2
  type: string
- description: City
  name: city
  type: string
- description: State
  name: state
  type: string
- description: Postal code
  name: postalCode
  type: string
- description: Alpha-3 ISO 3166-1 country code
  name: country
  type: string
- description: Email address
  name: email
  type: string
- description: Phone number
  name: phone
  type: string
- description: Payment card number
  name: pan
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-loyalty-insurance-submit-claim-user-data-schema.json
slug: mastercard-loyalty-insurance-submit-claim-user-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubmitClaimUserData\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name\"\n    },\n    \"addressLine1\": {\n      \"type\": \"string\",\n      \"description\": \"Address line 1\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\",\n      \"description\": \"Address line 2\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal code\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Alpha-3 ISO 3166-1 country code\"\n    },\n    \"email\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Email address\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number\"\n    },\n    \"pan\": {\n      \"type\": \"string\",\n      \"description\": \"Payment card number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-loyalty-insurance-submit-claim-user-data-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: SubmitClaimUserData
---
