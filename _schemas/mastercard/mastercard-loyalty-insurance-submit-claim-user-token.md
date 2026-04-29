---
description: ''
layout: schema
name: SubmitClaimUserToken
properties_list:
- description: Encrypted user data token to be used in the generated url that redirects the cardholder to the target website to submit a new claim.
  name: token
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-loyalty-insurance-submit-claim-user-token-schema.json
slug: mastercard-loyalty-insurance-submit-claim-user-token
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubmitClaimUserToken\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"Encrypted user data token to be used in the generated url that redirects the cardholder to the target website to submit a new claim.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-loyalty-insurance-submit-claim-user-token-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: SubmitClaimUserToken
---
