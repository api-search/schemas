---
description: Configuration details for an Issuer.
layout: schema
name: IssuerConfiguration
properties_list:
- description: Comma separated account range must be between 4 and 8 supported by an Issuer.
  name: supportedAccountRange
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
schema_file: json-schema/mastercard-carbon-calculator-experience-issuer-configuration-schema.json
slug: mastercard-carbon-calculator-experience-issuer-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IssuerConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"Configuration details for an Issuer.\",\n  \"properties\": {\n    \"supportedAccountRange\": {\n      \"type\": \"string\",\n      \"description\": \"Comma separated account range must be between 4 and 8 supported by an Issuer.\"\n    },\n    \"privacyNoticeURL\": {\n      \"type\": \"string\",\n      \"description\": \"Privacy Notice URL.\"\n    },\n    \"termsAndConditionURL\": {\n      \"type\": \"string\",\n      \"description\": \"Terms and conditions URL for the given user.\"\n    },\n    \"optOutURL\": {\n      \"type\": \"string\",\n      \"description\": \"Opt out URL for the given user.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-carbon-calculator-experience-issuer-configuration-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: IssuerConfiguration
---
