---
description: ''
layout: schema
name: IdentityRisk
properties_list:
- description: A comprehensive 0-500 score associated with the individual's identity.
  name: score
  type: integer
- description: 'Reason code explanation value for the identity risk score based on data provided. Possible values are: * High Severity : AA-AP * Medium Severity : JA-JF * Low Severity : RA-RP'
  name: reasonCode
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-identity-risk-schema.json
slug: mastercard-identity-insights-for-transactions-identity-risk
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IdentityRisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"score\": {\n      \"type\": \"integer\",\n      \"description\": \"A comprehensive 0-500 score associated with the individual's identity.\"\n    },\n    \"reasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"Reason code explanation value for the identity risk score based on data provided. Possible values are: * High Severity : AA-AP * Medium Severity : JA-JF * Low Severity : RA-RP\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-identity-risk-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: IdentityRisk
---
