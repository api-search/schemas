---
description: Successful user enrollment response
layout: schema
name: UserReference
properties_list:
- description: Last 4 digits of a full payment card number which were provided as enrollment request.
  name: cardNumberLastFourDigits
  type: string
- description: Status of the user on Carbon Calculator Experience API. Possible values are ACTIVE and INACTIVE.
  name: status
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-carbon-calculator-experience-user-reference-schema.json
slug: mastercard-carbon-calculator-experience-user-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserReference\",\n  \"type\": \"object\",\n  \"description\": \"Successful user enrollment response\",\n  \"properties\": {\n    \"cardNumberLastFourDigits\": {\n      \"type\": \"string\",\n      \"description\": \"Last 4 digits of a full payment card number which were provided as enrollment request.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the user on Carbon Calculator Experience API. Possible values are ACTIVE and INACTIVE.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-carbon-calculator-experience-user-reference-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: UserReference
---
