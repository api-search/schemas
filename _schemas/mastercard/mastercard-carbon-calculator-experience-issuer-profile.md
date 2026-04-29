---
description: Information about an Issuer as available on the server.
layout: schema
name: IssuerProfile
properties_list:
- description: Unique Issuer identifier from the Mastercard Developer Portal.
  name: clientId
  type: string
- description: Unique Issuer identifier assigned by Mastercard which remains the same across all Mastercard systems.
  name: customerId
  type: string
- description: Comma separated account range must be between 4 and 8 supported by an Issuer.
  name: supportedAccountRange
  type: string
- description: Status of an Issuer on the server. Possible values are Active and Suspended.
  name: status
  type: string
- description: Privacy Notice URL.
  name: privacyNoticeURL
  type: string
- description: Terms and conditions URL for the given user.
  name: termsAndConditionURL
  type: string
- description: Opt out URL for the given user.
  name: optOutURL
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-carbon-calculator-experience-issuer-profile-schema.json
slug: mastercard-carbon-calculator-experience-issuer-profile
source_filename: mastercard-carbon-calculator-experience-issuer-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IssuerProfile\",\n  \"type\": \"object\",\n  \"description\": \"Information about an Issuer as available on the server.\",\n  \"properties\": {\n    \"clientId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Issuer identifier from the Mastercard Developer Portal.\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Issuer identifier assigned by Mastercard which remains the same across all Mastercard systems.\"\n    },\n    \"supportedAccountRange\": {\n      \"type\": \"string\",\n      \"description\": \"Comma separated account range must be between 4 and 8 supported by an Issuer.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of an Issuer on the server. Possible values are Active and Suspended.\"\n    },\n    \"privacyNoticeURL\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Privacy Notice URL.\"\n    },\n    \"termsAndConditionURL\": {\n      \"type\": \"string\",\n      \"description\": \"Terms and conditions URL for the given user.\"\n    },\n    \"optOutURL\": {\n      \"type\": \"string\",\n      \"description\": \"Opt out URL for the given user.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-carbon-calculator-experience-issuer-profile-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: IssuerProfile
---
